# <a name="get-a-site-resource"></a>Obter um recurso de site

Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.

[site]: ../resources/site.md

Um **site** é endereçado para ser um identificador exclusivo que é uma ID composta dos seguintes valores:

* Hostname do conjunto de sites (contoso.sharepoint.com)
* ID exclusiva do conjunto de sites (guid)
* ID exclusiva do site (guid)

Também é um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:

* `/sites/root`: O site raiz do locatário.
* `/groups/{group-id}/sites/root`: O site da equipe do grupo.

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes escopos é necessário para executar esta solicitação:

* Sites.Read.All
* Sites.ReadWrite.All

## <a name="get-the-tenants-root-site"></a>Obter o site raiz do locatário

Para acessar o site raiz do SharePoint dentro de um locatário:

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>Acesse um site pela URL relativa do servidor

Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>Acesse um site de equipe do grupo

Para acessar o site de equipe de um [grupo](../resources/group.md):

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
