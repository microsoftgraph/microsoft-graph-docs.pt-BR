---
title: 'accessPackageAssignmentRequest: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackageassignmentrequest filtrados no usuário de entrada.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1fd32f90432c081c353a3455eddc83af0de6ee7e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098229"
---
# <a name="accesspackageassignmentrequest-filterbycurrentuser"></a>accessPackageAssignmentRequest: filterByCurrentUser
Namespace: microsoft.graph


No [Azure AD Entitlement Management](../resources/entitlementmanagement-overview.md), recupere uma lista de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) filtrados no usuário de entrada.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignmentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|accessPackageAssignmentRequestFilterByCurrentUserOptions|A lista de opções de usuário que podem ser usadas para filtrar na lista de solicitações de atribuição de pacote de acesso. Os valores possíveis são `target` `createdBy` , , `approver` .|

- `target` é usado para obter os `accessPackageAssignmentRequest` objetos em que o usuário inscreva é o destino. A lista resultante inclui todas as solicitações de atribuição, atuais e expiradas, que foram solicitadas pelo chamador ou pelo chamador, em todos os catálogos e pacotes de acesso.

- `createdBy` é usado para obter `accessPackageAssignmentRequest` os objetos criados pelo usuário in-locar. A lista resultante inclui todas as solicitações de atribuição que o chamador criou para si ou em nome de outras pessoas, como no caso de atribuição direta do administrador, em todos os catálogos e pacotes de acesso.

- `approver` é usado para obter os objetos em que o usuário inscreve `accessPackageAssignmentRequest` é um aprovador permitido para a solicitação. A lista resultante inclui as solicitações de atribuição em estado, em todos os catálogos e pacotes de acesso, que precisam de uma decisão `pending` do chamador.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` [coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests/filterByCurrentUser(on='target')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackageassignmentrequest-filterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackageassignmentrequest-filterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "46c1410d-ef96-44c5-ae9c-a577d014fe0e",
      "requestType": "adminAdd",
      "state": "delivered",
      "status": "Delivered",
      "createdDateTime": "2021-01-19T20:02:23.907Z",
      "completedDate": "2021-01-19T20:02:40.97Z",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```


