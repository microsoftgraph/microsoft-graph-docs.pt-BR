---
title: Obter governançaRoleDefinition
description: Recupere as propriedades e as relações de um governanceRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c42eee6a55eed75674f2f53563898dbe9d5e71e7
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350661"
---
# <a name="get-governanceroledefinition"></a>Obter governançaRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um [governanceRoleDefinition](../resources/governanceroledefinition.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Recursos do Azure

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Grupos

|Tipo de permissão | Permissões |
|:-------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application | PrivilegedAccess.Read.AzureADGroup |

Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso, à qual a [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método não **dá suporte** aos [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|


## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.
## <a name="example"></a>Exemplo
Este exemplo mostra como obter detalhes da definição de função DNS Zone Contributor na assinatura Wingtip Toys - Prod.
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


