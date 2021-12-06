# LearnAngular

<H5>Building Nested Components (Child component)-</H5>
**HOW TO IDENTIFY CHILD COMPOENT:
1- It will placed inside subfolder of the parent component.
2-Child comp uses logic from parent
-----------------------------------------------------------
**HOW TO PASS DATA TO NESTED COMPONENT USING @INPUT-
1-@Input decorator is used to pass data to nested component.
2-@Input binds the expression into the directive.

      APP
      /  \
     /     \
 Login   Patient
          /  \
         /    \ 
      Task    Observation @Input() : Pat_info :Object
-------------------------------------------------------------      
**HOW TO PASS DATA FROM NESTED COMPONENT USING @OUTPUT-    
1-Parent is updated by Child using @Output
2-It is used if parent-child hierarchy is small.
3- Notifies the parent component about the changes.

@OUTPUT AND @EventEmitter go together
1-the parent is notified by this.
2- is used to emit the data frommchild to parent component.
3-Emits an event to parent using event binding.
------------------------------------------------------------
** SPECIAQL DECORATOR- ViewChild:
1- access child component directly from parent(done using reference)
2-used for configuring view query
3-used to select specific element form view
4- requires inputs like selectors.read,write eetc.
5-syntax- 
   @ViewChild(selector {read:readValue,static:staticValue}) property;
