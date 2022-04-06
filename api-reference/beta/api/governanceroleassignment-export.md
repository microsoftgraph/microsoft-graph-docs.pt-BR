---
title: Exportar governançaRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests `application/octet-stream`no formato , que pode ser analisado como um arquivo .csv no navegador.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: japere
ms.openlocfilehash: c7f4aada8b5dd7d31b9dcce99112ddb8d3ec2682
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64508606"
---
# <a name="export-governanceroleassignmentrequests"></a>Exportar governançaRoleAssignmentRequests

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Recupere uma coleção [de governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) `application/octet-stream`no formato , que pode ser analisado como um arquivo .csv no navegador.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Recursos do Azure

| Tipo de permissão | Permissions |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Microsoft Azure AD

| Tipo de permissão | Permissions |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Grupos

|Tipo de permissão | Permissions |
|:-------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | PrivilegedAccess.Read.AzureADGroup |


## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso
    
>**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Exportar uma coleção [de governançaRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de minha
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um conteúdo do tipo `application/octet-stream`.

## <a name="example"></a>Exemplo
Este exemplo salva todas as atribuições de função como um arquivo .csv na assinatura Wingtip Toys - Prod. 

##### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


