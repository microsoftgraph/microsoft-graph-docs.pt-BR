---
title: Obter direitosManagementSettings
description: Recupere as propriedades do objeto entitlementManagementSettings.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a12f5694b58ea774c60d994db21d99b2c7faa9f9
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242197"
---
# <a name="get-entitlementmanagementsettings"></a>Obter direitosManagementSettings

Namespace: microsoft.graph

Recupere as propriedades de [um objeto entitlementManagementSettings.](../resources/entitlementmanagementsettings.md)

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
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não é compatível com os Parâmetros de Consulta OData para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [requested entitlementManagementSettings](../resources/entitlementmanagementsettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_entitlementmanagementsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/settings
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "singleton",
  "externalUserLifecycleAction": "blockSignInAndDelete",
  "durationUntilExternalUserDeletedAfterBlocked": "P4D"
}
```

