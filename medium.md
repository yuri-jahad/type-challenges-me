# typescript-progress-challenge

## Medium

### [2] GetReturnType

- **Statut** : ✅ solved
- **Date** : 11/10/2025
- **Solution** :

```typescript
type MyReturnType<T extends (...args: any[]) => any> = T extends (...args: any[]) => infer R ? R : never
```
### [3] Omit

- **Statut** : ✅ solved
- **Date** : 11/10/2025
- **Solution** :

```typescript
type MyOmit<T, K extends keyof T> = {
  [key in keyof T as key extends K ? never: key]  : T[key]
}
```