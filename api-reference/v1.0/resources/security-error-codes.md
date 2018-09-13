# <a name="security-api-error-responses"></a>Respostas de erros da API de segurança

Erros da API de segurança do Microsoft Graph são retornados usando códigos de status padrão HTTP e são entregues como cabeçalho de aviso.

A API de segurança é um serviço federado que recebe várias respostas de todos os provedores de dados. Quando um erro HTTP é recebido pela API de segurança, ele retornará um cabeçalho de aviso no seguinte formato: <!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Este cabeçalho de aviso será enviado de volta para os clientes somente quando um dos provedores de dados retornar um código de erro diferente de 2xx ou 404. Por exemplo:

- HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não for concedido.
- Se um provedor não responde a tempo, HttpStatusCode.GatewayTimeout (504) é retornado no cabeçalho de aviso.
- Se ocorrer um erro interno no provedor, HttpStatusCode.InternalServerError (500) é usado no cabeçalho de aviso.

Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho do aviso porque esses são códigos esperados de êxito ou quando os dados não são encontrados, respectivamente. Em um sistema federado, um erro 404 não encontrado é esperado, pois muitas vezes os dados são conhecidos por um ou vários provedores, mas não por todos.

## <a name="example"></a>Exemplo

Um usuário solicita `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Como 404 e 200 são condições esperadas, o cabeçalho do aviso contém o seguinte: 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitems, para que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.

## <a name="see-also"></a>Confira também

Se você estiver tendo problemas com autorização, confira nossa [postagem no blog](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).
