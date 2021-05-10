---
title: 'accessPackage: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackage filtrados no usuário de entrada.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4212c06606c6363a31e64dee7da820d93ea13fa
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299011"
---
# <a name="accesspackage-filterbycurrentuser"></a>accessPackage: filterByCurrentUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackage](../resources/accesspackage.md) filtrados no usuário de entrada.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|[accessPackageFilterByCurrentUserOptions](../resources/accesspackage-accesspackagefilterbycurrentuseroptions.md)|A lista de opções de usuário atuais que podem ser usadas para filtrar na lista de pacotes de acesso.|

- `allowedRequestor` é usado para obter os objetos para os quais o usuário interno tem permissão `accessPackage` para enviar solicitações de acesso. A lista resultante inclui todos os pacotes de acesso que podem ser solicitados pelo chamador em todos os catálogos.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [accessPackage](../resources/accesspackage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
O exemplo a seguir obtém os pacotes de acesso que podem ser solicitados pelo usuário interno.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterByCurrentUser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')
```


### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
            "@odata.type": "#microsoft.graph.accessPackage",
            "id": "d378b3b7-b42a-445a-8780-2841194f777e",
            "catalogId": "eb0f5e12-484d-4545-8ae1-fb1dfc28ab3c",
            "displayName": "Sales resources",
            "description": "Resources needed by the Sales department.",
            "isHidden": false,
            "isRoleScopesVisible": false,
            "createdBy": "TestGA@example.com",
            "createdDateTime": "2021-01-26T22:30:57.37Z",
            "modifiedBy": "TestGA@example.com",
            "modifiedDateTime": "2021-01-26T22:30:57.37Z"
        }
    ]
}
```

