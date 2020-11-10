---
title: Listar activityStatistics
description: Obtenha uma coleção de objetos activityStatistics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: ba1fb1fb18b3791b43d17ffeb11fadf7edd608aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952498"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="a0f08-103">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="a0f08-103">List activityStatistics</span></span>

<span data-ttu-id="a0f08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0f08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0f08-105">Obtenha uma coleção de [activityStatistics](../resources/activitystatistics.md) para um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="a0f08-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0f08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0f08-106">Permissions</span></span>

<span data-ttu-id="a0f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0f08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0f08-109">Permission type</span></span>                        | <span data-ttu-id="a0f08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0f08-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0f08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0f08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0f08-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="a0f08-112">Analytics.Read</span></span> |
| <span data-ttu-id="a0f08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0f08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0f08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0f08-114">Not supported.</span></span> |
| <span data-ttu-id="a0f08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0f08-115">Application</span></span>                            | <span data-ttu-id="a0f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0f08-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0f08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0f08-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0f08-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0f08-118">Optional query parameters</span></span>

<span data-ttu-id="a0f08-119">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0f08-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0f08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f08-120">Request headers</span></span>

| <span data-ttu-id="a0f08-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a0f08-121">Name</span></span>      |<span data-ttu-id="a0f08-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0f08-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0f08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0f08-123">Authorization</span></span> | <span data-ttu-id="a0f08-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a0f08-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0f08-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f08-125">Request body</span></span>

<span data-ttu-id="a0f08-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0f08-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0f08-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0f08-127">Response</span></span>

<span data-ttu-id="a0f08-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [activityStatistics](../resources/activitystatistics.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0f08-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0f08-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0f08-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0f08-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0f08-130">Request</span></span>

<span data-ttu-id="a0f08-131">Veja a seguir um exemplo de uma solicitação de todas as estatísticas de atividade relacionadas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a0f08-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0f08-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0f08-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="a0f08-133">C#</span><span class="sxs-lookup"><span data-stu-id="a0f08-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0f08-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0f08-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0f08-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0f08-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0f08-136">Java</span><span class="sxs-lookup"><span data-stu-id="a0f08-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitystatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0f08-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0f08-137">Response</span></span>

<span data-ttu-id="a0f08-138">Veja a seguir um exemplo de uma resposta com todas as estatísticas de atividade relacionadas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a0f08-138">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="a0f08-139">Essa resposta mostra apenas o primeiro dia das atividades de uma semana para reduzir a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0f08-139">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="a0f08-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0f08-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


