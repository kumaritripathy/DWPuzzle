1. we can use async pipe in this case to iterate data in html.

2. we can define store globally,no need to add in ngOninit.
   books$ = this.store.select(getAllBooks)

3. This pipe can handle subscription and unsubscription both.
    <div *ngFor="let book of books$|async">{{book?.name}}</div>   

   