---
title: 'organization: activateService'
description: Ativa um serviço para uma organização.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6008b7f5a597af5ac65b349af22879b9db1255f4
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109073"
---
# <a name="organization-activateservice"></a>organization: activateService

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ative um serviço para uma organização.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para ativar um serviço para uma organização, o  solicitante precisa ter a função administrador da empresa com as seguintes permissões.

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
| :--- | :--- |
| Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All|
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Directory.ReadWrite.All|


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto activateService.](../resources/activateService.md)
Você deve definir **o serviço** ou (**servicePlanId** _e_ **skuId**) para que essa ação seja válida.

| Propriedade         | Tipo         | Descrição                           |
| ----------------- | ------------ | ------------------------------------- |
| service| Cadeia de caracteres | O nome do serviço a ser ativado. |
| servicePlanId | Guid | O identificador de plano do plano de serviço a ser ativado. |
| skuId | Guid | O identificador SKU do plano de serviço. |

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "organization_activateservice"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{:organizationId}/activateService
Content-Type: application/json

{
    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900",
    "servicePlanId": "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```