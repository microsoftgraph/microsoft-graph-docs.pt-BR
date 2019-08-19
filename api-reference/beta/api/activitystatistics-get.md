---
title: Obter activityStatistics
description: Recupere as propriedades de um objeto activityStatistics para um usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d538b6389cd2a85768c15679d29d2fc9c11a0ff9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460805"
---
# <a name="get-activitystatistics"></a>Obter activityStatistics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter as propriedades de um objeto [activityStatistics](../resources/activitystatistics.md) para um usuário.

Você pode obter as propriedades de um tipo de [activityStatistics](../resources/activitystatistics.md) para o usuário especificado e o intervalo de datas. Você pode especificar o tipo de estatísticas e o intervalo de datas usando o formato com suporte da [Propriedade Activity ID](../resources/activitystatistics.md#activity-id-property) para `id` na consulta.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Analytics. Read |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e o tipo solicitado de estatísticas de atividade, que é um dos seguintes recursos derivados de [ActivityStatistics](../resources/activitystatistics.md): {[Call](../resources/callactivitystatistics.md), [chat](../resources/chatactivitystatistics.md), [email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), e [reunião](../resources/meetingactivitystatistics.md)}.

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

O exemplo a seguir solicita estatísticas do tipo emailActivityStatistics do usuário conectado, para o intervalo de datas entre 2019-06-16 e 2019-06-17. Para obter mais informações sobre o formato de propriedade de ID geral, consulte [Activity ID Property](../resources/activitystatistics.md#activity-id-property).


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta que obtém as estatísticas de atividade de um usuário conectado para uma atividade e um dia específicos.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics/$entity",
    "@odata.type": "#microsoft.graph.emailActivityStatistics",
    "activity": "Email",
    "startDate": "2019-06-16",
    "endDate": "2019-06-17",
    "id": "email_2019-06-16_2019-06-17",
    "timeZoneUsed": "Pacific Standard Time",
    "duration": "PT0S",
    "afterHours": "PT0S",
    "readEmail": "PT0S",
    "sentEmail": "PT0S"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityStatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
