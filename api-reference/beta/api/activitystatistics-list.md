---
title: Listar activityStatistics
description: Obtenha uma coleção de objetos activityStatistics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0b6c499bf86041e3f071977370e898b1471c3755
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441785"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="f573e-103">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="f573e-103">List activityStatistics</span></span>

<span data-ttu-id="f573e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f573e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f573e-105">Obtenha uma coleção de [activityStatistics](../resources/activitystatistics.md) para um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="f573e-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="f573e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f573e-106">Permissions</span></span>

<span data-ttu-id="f573e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f573e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f573e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f573e-109">Permission type</span></span>                        | <span data-ttu-id="f573e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f573e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f573e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f573e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f573e-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="f573e-112">Analytics.Read</span></span> |
| <span data-ttu-id="f573e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f573e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f573e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f573e-114">Not supported.</span></span> |
| <span data-ttu-id="f573e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f573e-115">Application</span></span>                            | <span data-ttu-id="f573e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f573e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f573e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f573e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f573e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f573e-118">Optional query parameters</span></span>

<span data-ttu-id="f573e-119">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f573e-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f573e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f573e-120">Request headers</span></span>

| <span data-ttu-id="f573e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f573e-121">Name</span></span>      |<span data-ttu-id="f573e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f573e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f573e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f573e-123">Authorization</span></span> | <span data-ttu-id="f573e-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f573e-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f573e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f573e-125">Request body</span></span>

<span data-ttu-id="f573e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f573e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f573e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f573e-127">Response</span></span>

<span data-ttu-id="f573e-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [activityStatistics](../resources/activitystatistics.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f573e-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f573e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f573e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f573e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f573e-130">Request</span></span>

<span data-ttu-id="f573e-131">Veja a seguir um exemplo de uma solicitação de todas as estatísticas de atividade relacionadas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f573e-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="f573e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f573e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="f573e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f573e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f573e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f573e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f573e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f573e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f573e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f573e-136">Response</span></span>

<span data-ttu-id="f573e-137">Veja a seguir um exemplo de uma resposta com todas as estatísticas de atividade relacionadas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f573e-137">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="f573e-138">Essa resposta mostra apenas o primeiro dia das atividades de uma semana para reduzir a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f573e-138">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="f573e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f573e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics",
    "value": [
        {
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
        },
        {
            "@odata.type": "#microsoft.graph.meetingActivityStatistics",
            "activity": "Meeting",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "meeting_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S",
            "organized": "PT0S",
            "recurring": "PT0S",
            "long": "PT0S",
            "conflicting": "PT0S",
            "multitasking": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.focusActivityStatistics",
            "activity": "Focus",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "focus_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.chatActivityStatistics",
            "activity": "Chat",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "chat_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.callActivityStatistics",
            "activity": "Call",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "call_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List activitystatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
