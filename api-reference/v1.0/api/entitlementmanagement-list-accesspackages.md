---
title: Listar accessPackages
description: Recupere uma lista de objetos accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 11e21b61322507e7791837fc52557d4854c645e9
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242260"
---
# <a name="list-accesspackages"></a>Listar accessPackages

Namespace: microsoft.graph


Recupere uma lista de [objetos accessPackage.](../resources/accesspackage.md)  A lista resultante inclui todos os pacotes de acesso que o chamador tem acesso para ler, em todos os catálogos.

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
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos `$select` `$filter` parâmetros de consulta E OData para ajudar a personalizar a resposta. Por exemplo, para recuperar as políticas de pacote de acesso para cada pacote de acesso, adicione `$expand=accessPackageAssignmentPolicies` . Para pesquisar pacotes de acesso com um nome específico, inclua um filtro como `$filter=contains(tolower(displayName),'team')` na consulta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackage](../resources/accesspackage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackage",
      "id": "114d3459-3459-114d-5934-4d1159344d11",
      "displayName": "Access package for testing",
      "description": "Sample access package",
      "isHidden": false,
      "createdDateTime": "2019-01-27T18:19:50.74Z",
      "modifiedDateTime": "2019-01-27T18:19:50.74Z"
    }
  ]
}
```


