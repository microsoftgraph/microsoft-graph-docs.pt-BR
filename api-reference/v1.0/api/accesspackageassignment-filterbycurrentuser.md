---
title: 'accessPackageAssignment: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackageassignment filtrados no usuário de entrada.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9ed084f91e84d288ad8ea3d7d07ebaa4b32ffa9e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242169"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a>accessPackageAssignment: filterByCurrentUser
Namespace: microsoft.graph


No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) filtrados no usuário de entrada.

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
GET /identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|accessPackageAssignmentFilterByCurrentUserOptions|A lista de opções de usuário que podem ser usadas para filtrar na lista de atribuições do pacote de acesso.|

- `target` é usado para obter os `accessPackageAssignment` objetos em que o usuário inscreva é o destino. A lista resultante inclui todas as atribuições, atuais e expiradas, para o chamador em todos os catálogos e pacotes de acesso.

- `createdBy` é usado para obter `accessPackageAssignment` os objetos criados pelo usuário in-locar. A lista resultante inclui todas as atribuições que o chamador criou para si ou em nome de outras pessoas, como no caso de atribuição direta do administrador, em todos os catálogos e pacotes de acesso.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` [coleção accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.

Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade na resposta que contém uma URL para `@odata.nextLink` a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL em `@odata.nextLink` cada resposta, até que todos os resultados sejam retornados. Para obter mais informações, [consulte paging Microsoft Graph data in your app](/graph/paging).

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='target')
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "null",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```

