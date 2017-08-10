# <a name="list-serviceconfigurationrecords"></a>Listar serviceConfigurationRecords

Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para ativar os serviços do domínio.

Use a lista retornada para adicionar registros para ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a>Resposta
Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->