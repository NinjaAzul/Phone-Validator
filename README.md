# Phone-Validator

```
export const phoneValidator = (str?: string): boolean => {
  if (!str) return false;

  return (
    new RegExp(/^(\d{10,11})$/).test(str.replace(/\D/g, '')) ||
    new RegExp(phoneRegEx).test(str.replace(/\D/g, ''))
  );
};
```
