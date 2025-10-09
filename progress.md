# typescript-progress-challenge

## Easy

### [4] Pick

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type MyPick<T, K extends keyof T> = {
  [key in K]: T[key]
}
```

### [7] ReadOnly

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type MyReadonly<T> = {
  readonly [K in keyof T]: T[K]
}
```
