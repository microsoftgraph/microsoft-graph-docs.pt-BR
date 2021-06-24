---
title: Obter userInsightsSettings
description: Recupere as propriedades de um objeto userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 11796934c9ea2edd7a5c3905604671f29604f973
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109059"
---
# <a name="get-userinsightssettings"></a>Obter userInsightsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter as configurações de privacidade personalizáveis pelo usuário [para o itemInsights](../resources/iteminsights.md) e informações do horário [de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read, User.ReadWrite |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |


## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

>**Observação:** As solicitações com um ou são acessíveis apenas pelo usuário ou por um usuário com as permissões `userId` `userPrincipalName` User.ReadWrite.All. Para saber mais, confira [permissões](/graph/permissions-reference).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userInsightsSettings](../resources/userinsightssettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação para obter informações de item do usuário e configurações de insights de horários de reunião.

<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```http
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "get_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": true
}
```


