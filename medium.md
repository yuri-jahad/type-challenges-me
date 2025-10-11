# typescript-progress-challenge

## Medium

### [2] GetReturnType

- **Statut** : ✅ solved
- **Date** : 09/10/2025
- **Solution** :

```typescript
type MyReturnType<T extends (...args: any[]) => any> = T extends (...args: any[]) => infer R ? R : never
```