---
title: 'user: activateServicePlan'
description: Ative um plano de serviço com um `servicePlanId` determinado e para um determinado `skuId` usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 70849865237a82f4a0bb5fcee22263291627c21d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578851"
---
# <a name="user-activateserviceplan"></a>user: activateServicePlan

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ative um plano de serviço com um `servicePlanId` determinado e para um determinado `skuId` usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
| :--- | :--- |
| Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
| :--- | :--- |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro:

| Parâmetro | Tipo | Descrição |
| :--- | :--- | :--- |
| servicePlanId | Guid | PlanId do ServicePlan a ser ativado. |
| skuId | Guid | SkuId de SKU o plano de serviço está em. |

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "user_activateserviceplan"
}
-->

``` http
POST https://graph.microsoft.com/beta/me/activateServicePlan
Content-type: application/json
Content-length: 115

{
  "servicePlanId": "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
  "skuId": "465a2a90-5e59-456d-a7b8-127b9fb2e484"
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
