---
title: Listar serviceManagementDetails
description: Obtenha uma lista dos objetos delegatedAdminServiceManagementDetail e suas propriedades.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: c61167f61ff0caf04dee02d43e82d855665c9679
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704237"
---
# <a name="list-servicemanagementdetails"></a>Listar serviceManagementDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos delegatedAdminServiceManagementDetail](../resources/delegatedAdminServiceManagementDetail.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminCustomers/{delegatedAdminCustomerId}/serviceManagementDetails
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não dá suporte a parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters). 

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de objetos [delegatedAdminServiceManagementDetail](../resources/delegatedAdminServiceManagementDetail.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_delegatedAdminServiceManagementDetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001/serviceManagementDetails
```

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminServiceManagementDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001/serviceManagementDetails",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "fa5fa04e-13df-4b7c-9e99-92573ba1fa55",
      "serviceManagementUrl": "https://aad.portal.azure.com/contoso.onmicrosoft.com",
      "serviceName": "Azure Active Directory"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "5d0273c3-0f0e-4e00-90e8-e792c8860fb5",
      "serviceManagementUrl": "https://lighthouse.microsoft.com",
      "serviceName": "Microsoft 365 Lighthouse"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "2b565abc-b0de-4974-97c0-bed0abb14a0f",
      "serviceManagementUrl": "https://businesscentral.dynamics.com/55beae45-27a6-4e7a-8c7c-2eae70816cfa/admin",
      "serviceName": "Dynamics 365 Business Central"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "ce0b42f4-bfde-4abe-a5f7-add83f104b23",
      "serviceManagementUrl": "https://admin.teams.microsoft.com/?delegatedOrg=contoso.onmicrosoft.com",
      "serviceName": "Teams"
    }
  ]
}
```

