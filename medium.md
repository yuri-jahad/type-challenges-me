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
### [8] Readonly2

- **Statut** : ✅ solved
- **Date** : 12/10/2025
- **Solution** :

```typescript
type MyReadonly2<T, K extends keyof T = keyof T> = 
  Omit<T, K> & Readonly<Pick<T, K>>
```
g