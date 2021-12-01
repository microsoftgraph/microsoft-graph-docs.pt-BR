---
title: Listar accessPackageCatalogs
description: Recupere uma lista de objetos accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 67547de703081633ff953f0baffe0cfcc40d94aa
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242229"
---
# <a name="list-catalogs"></a>Listar catálogos

Namespace: microsoft.graph

Recupere uma lista de [objetos accessPackageCatalog.](../resources/accesspackagecatalog.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/catalogs
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte `$select` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$expand` a resposta. Por exemplo, para recuperar os pacotes de acesso em cada catálogo, `$expand=accessPackages` inclua na consulta. Para pesquisar catálogos de pacotes de acesso com um nome específico, inclua um filtro como `$filter=contains(tolower(displayName),'staff')` na consulta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_accesspackagecatalog"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageCatalog)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
      "displayName": "Access package catalog for testing",
      "description": "Sample access package catalog",
      "catalogType": "userManaged",
      "state": "published",
      "isExternallyVisible": false,
      "createdDateTime": "2019-01-27T18:19:50.74Z",
      "modifiedDateTime": "2019-01-27T18:19:50.74Z"
    }
  ]
}
```



