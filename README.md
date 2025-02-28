Rotas - Projeto EasyCar

-------------------------------------------------

[x]Consultar  se existe  corrida pendente (hoje) para o usuario logado
    GET -> /rides
    Filtros:passenger_user_id, pickup_date, ride_id, driver_user_id, status

[x]Cadastrar novas carona
    POST -> /rides

[x]Cancelar  um pedido  de carona (excluir o pedido)
    DELETE -> /rides/123

[x]Finalizar uma carona  que foi concluida
    PUT -> /rides/123/finish
    Body: passenger_user_id

[x]Consultar as corridas  para o motorista (corrida dele + corridas pendentes)
    GET -> /rides/drivers/456

[x]Consultar todos os dados  de uma determinada corrida
    GET ->/rides/123

[x]Motorista  aceitar  uma carona
    PUT -> /rides/123/accept
    Body:driver_user_id

[x]Motorista cancelar uma carona
    PUT -> /rides/123/cancel


Bussiness Rules (Regras de Negocio)
-------------------------------------------------------------------

[X] O usuario  so pode  pedir uma carona por vez

[x] O motorista  só pode  aceitar  uma carona por vez

#   E a s y C a r  
 