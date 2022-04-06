---
title: Listar assignmentPolicies
description: Listar os objetos accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82de66f4eac1095374177eff848ea4e6b67d1540
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608239"
---
# <a name="list-assignmentpolicies"></a>Listar assignmentPolicies
Namespace: microsoft.graph

No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), recupere uma lista de [objetos accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) . Se o usuário delegado estiver em uma função de diretório, a lista resultante incluirá todas as políticas de atribuição que o chamador tem acesso à leitura, em todos os catálogos e pacotes de acesso. Se o usuário delegado for um gerenciador de pacotes de acesso ou proprietário de catálogo, ele deverá recuperar as políticas dos pacotes de acesso que podem ser [lidos com accessPackages](entitlementmanagement-list-accesspackages.md) `$expand=accessPackageAssignmentPolicies` de lista incluindo como parâmetro de consulta.

## <a name="permissions"></a>Permissions

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
GET /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns dos `$filter`parâmetros de consulta , `$select`e `$expand` OData para ajudar a personalizar a resposta. Por exemplo, para recuperar uma política de atribuição de pacote de acesso com um nome de exibição especificado, inclua `$filter=displayName eq 'Employee sales support'` na consulta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "displayName": "All Users",
      "description": "All users can request for access to the directory."
    }
  ]
}
```


