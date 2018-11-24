# <a name="microsoft-graph-security-api-error-responses"></a>Respostas de erros de API de segurança do Microsoft Graph

Erros na API de segurança do Microsoft Graph no Microsoft Graph são retornados usando o código de status HTTP 206 parcial conteúdo padrão e são fornecidos por meio de um cabeçalho de aviso.

A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados. Quando um erro HTTP é recebido pelo API de segurança do Microsoft Graph, ele retornará um cabeçalho de aviso no seguinte formato:<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Este cabeçalho do aviso será enviado apenas para os clientes quando um dos provedores de dados retorna um código de erro que não seja 2xx ou 404. Por exemplo:

- HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não é concedido.
- Se um provedor de tempo limite, HttpStatusCode.GatewayTimeout (504) é retornado no cabeçalho do aviso.
- Se um erro interno do provedor acontecer, HttpStatusCode.InternalServerError (500) é usado no cabeçalho do aviso.

Se um provedor de dados retorna 2xx ou 404, ele não será mostrado no cabeçalho do aviso porque esses códigos esperados para o sucesso ou quando os dados não são encontrados respectivamente. Em um sistema federado, um 404 não encontrado é esperado como muitas vezes, os dados somente são conhecidos por um ou vários, mas nem todos os provedores.

## <a name="example"></a>Exemplo

Um usuário solicita `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Como 404 e 200 são condições esperadas, o cabeçalho do aviso contém o seguinte: 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitems, para que os usuários possam enumerar o cabeçalho do aviso e verificar todos os itens.

## <a name="see-also"></a>Confira também

Se você estiver tendo problemas com autorização, consulte nosso [postagem de blog](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).
