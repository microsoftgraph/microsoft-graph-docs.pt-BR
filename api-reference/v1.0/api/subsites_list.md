# <a name="enumerate-subsites-of-a-site"></a>Enumerar subsites de um site

Obtém uma coleção de subsites definido para um [site][].

[site]: ../resources/site.md

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes escopos é necessário para executar esta solicitação:

* Sites.Read.All
* Sites.ReadWrite.All

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

### <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Enumerate subsites"
} -->
