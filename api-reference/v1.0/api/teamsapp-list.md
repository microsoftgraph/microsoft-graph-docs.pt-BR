---
title: Listar teamsApp
description: Listar aplicativos do teams publicados no catálogo de aplicativos do locatário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3ad19981ac92f1320a3e9ac15137664453ebf3da
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808964"
---
# <a name="list-teamsapp"></a>Listar teamsApp

Namespace: microsoft.graph

Listar [aplicativos](../resources/teamsapp.md) publicados no catálogo de aplicativos do Microsoft Teams. Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

> **Observação:** Somente os administradores globais podem chamar esta API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:------------------------------------|
| Delegado (conta corporativa ou de estudante)     | AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte                       |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

`$expand=AppDefinitions`O uso retornará mais informações sobre o estado do aplicativo, como o **publishingstate**, que reflete o status de análise de envio de aplicativos e retorna se um aplicativo foi aprovado, rejeitado ou permanece em revisão. 

> **Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados. Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-applications-in-your-tenant"></a>Exemplo 1: listar todos os aplicativos em seu locatário

O exemplo a seguir lista todos os aplicativos que são específicos para o locatário.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>Exemplo 2: listar aplicativos com uma determinada ID

O exemplo a seguir lista os aplicativos com uma determinada ID.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a>Exemplo 3: listar aplicativos com uma determinada ID e retornar o estado de revisão de envio

O exemplo a seguir lista os aplicativos com uma determinada ID e expande **appDefinitions** para retornar o **publishingstate**, que reflete o estado de análise de envio do aplicativo. `Submitted` significa que a revisão está pendente, `published` significa que o aplicativo foi aprovado pelo administrador e `rejected` significa que o aplicativo foi rejeitado pelo administrador.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
                {

                    "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",

                    "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",

                    "azureADAppId": null,

                    "displayName": "Test App",

                    "version": "1.0.1",

                    "requiredResourceSpecificApplicationPermissions": [],

                    "publishingState": "published"

                  }
            ]
      }
    ]
  }
```
