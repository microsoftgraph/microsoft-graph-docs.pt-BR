---
title: Criar connectedOrganization
description: Crie uma nova connectedOrganization.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f1bedc5001ac9d52e16f537629d6a92e62960928
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242223"
---
# <a name="create-connectedorganization"></a>Criar connectedOrganization

Namespace: microsoft.graph


Crie um novo [objeto connectedOrganization.](../resources/connectedorganization.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto connectedOrganization.](../resources/connectedorganization.md)

Você pode especificar as seguintes propriedades ao criar **uma connectedOrganization**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da organização conectada. |
|description|Cadeia de caracteres|A descrição da organização conectada.|
|identitySources|[Coleção identitySource](../resources/identitysource.md)|Uma coleção com um elemento, a fonte de identidade inicial nesta organização conectada.|
|state|connectedOrganizationState|O estado de uma organização conectada define se as políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não. Os valores possíveis são: `configured` e `proposed`.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ],
  "state":"proposed"
}
```

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "35ff48a8-e9d8-4405-8425-0b23694287a4",
  "displayName": "Connected organization name",
  "description": "Connected organization description",
  "createdDateTime": "2021-11-10T01:13:15.541617Z",
  "modifiedDateTime": "2021-11-10T01:13:15.541617Z",
  "state": "proposed",
  "identitySources": []
}
```

