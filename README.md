RF  - Req. Funcionais
RNF - Req. Não funcionais
RN  - Regra de Negócio

POST /customers
  name, email, created_at, updated_at

  RF
    - Deve permitir cadstrar o cliente
    
  RN
    - Não pode ter um cliente com o mesmo email
    
POST /products
  name, price, quantity, created_at, updated_at
  
  RN
    - Não deve existir produtos com nomes duplicados
    
  RNF
    - Campo price: type -> decimal passando propriedads precision e acle
    
POST /orders
  orders: id, customer_id, created_at, updated_at
  orders_products: id, product_id, order_id, price, quantity, created_at, updated_at
  

