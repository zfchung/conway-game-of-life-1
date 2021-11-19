# conway-game-of-life-1

Practice OOP using TypeScript with Outside-In approach

Open-closed:

- Avoid having attributes that are public
- Avoid allowing application to change the attribute directly
- Avoid implementation leaking
- Use encapsulation (setter) so that the implementation can be encapsulated in setter();

```typescript
if (this.coordinateList[1][2].cell.isActive) {
    this.coordinateList[1][2].cell.isAlive = true;
}
```

```typescript
this.coordinateList[1][2].cell.setIsAlive(true);
```

```typescript
 public setIsAlive(value: boolean)
{
    if (this.isActive) {
        this.isAlive = value;
    }
}
```
