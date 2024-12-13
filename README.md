# QA Rest API Tests
This repository contains a Postman collection for API testing of the **QA Auto** application. The project involves testing in two environments (Production and Development) with automated validations for various API scenarios.
---

## 📚 Description

The test project includes the following API functionalities:
- User creation with unique data.
- Editing user profile (including avatar changes).
- Changing user password.
- Performing `logout` and `login` operations.
- Adding and deleting cars.
- Adding expenses to created cars.
- Negative testing for field validation.

---

## 📁 Structure

- **Collection:** Contains request groups organized by functionality.
- **Environments:** Separate files for Production and Development environments.
- **CSV file:** Input data for parameterized tests.

---

## 🛠️ Usage

1. **Import files:**
   - Collection (`.json` file).
   - Environments (`.json` files).
2. **Run tests:**
   - Select an environment (Production/Dev).
   - Use the `Run manually` mode to execute tests with all input data.

---

## 📜 Testing Instructions

### Environments
**Production:**
- [API Documentation](https://qauto.forstudy.space/api-docs/#/)
- Login: `guest`
- Password: `welcome2qauto`

**Development:**
- [API Documentation](https://qauto2.forstudy.space/api-docs/#/)
- Login: `guest`
- Password: `welcome2qauto`

---

### Key Tests
- **User creation:** Ensure uniqueness and verify `json schema`.
- **Profile editing:** Test all fields, including `dateBirth`.
- **Password change:** Verify `userId` consistency.
- **Expense addition:** Ensure the new value exceeds the previous one.

---

## ⚙️ Optimization

- Avoid duplicate code by using parameterization.
- One request can handle multiple validation scenarios.
- Tests are automatically executed for both environments (two iterations).

---

## 📊 Outputs

- Postman collection with scripts.
- Environment files (Production, Development).
- CSV file with test data.

---
