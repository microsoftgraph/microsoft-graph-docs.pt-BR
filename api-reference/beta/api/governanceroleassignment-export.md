---
title: Exportar governanceRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests no formato `application/octet-stream`, que pode ser analisado como um arquivo. csv no navegador.
localization_priority: Normal
ms.openlocfilehash: c01234ce4976d6f900530bdd06d31a4df8e325b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324154"
---
# <a name="export-governanceroleassignmentrequests"></a>Exportar governanceRoleAssignmentRequests

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato `application/octet-stream`, que pode ser analisado como um arquivo. csv no navegador.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess. ReadWrite. AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess. ReadWrite. AzureResources |


## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso
    
>**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de meus
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
Se tiver êxito, este método retornará `200 OK` um código de resposta e o `application/octet-stream`conteúdo do tipo.

## <a name="example"></a>Exemplo
Este exemplo salva todas as atribuições de função como um arquivo. csv na assinatura Wingtip Toys-prod. 

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
