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

### [11] TupleToObject

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type TupleToObject<T extends readonly any[]> = {
  [K in T[number]]: K
}
```
### [14] FirstOfArray

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type First<T extends any[]> = T extends [infer K, ...any[]] ? K : never
```
### [18] LengthOfTuple

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type Length<T extends readonly any[]> = T["length"] 
```
