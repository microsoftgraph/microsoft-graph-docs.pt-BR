---
title: Listar activityStatistics
description: Obter uma coleção de objetos activityStatistics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 422d6b3d03129d2e1c7169f3131c46fadc457e35
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048306"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="c106f-103">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="c106f-103">List activityStatistics</span></span>

<span data-ttu-id="c106f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c106f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c106f-105">Obter uma coleção [de activityStatistics](../resources/activitystatistics.md) para um usuário, para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="c106f-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="c106f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c106f-106">Permissions</span></span>

<span data-ttu-id="c106f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c106f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c106f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c106f-109">Permission type</span></span>                        | <span data-ttu-id="c106f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c106f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c106f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c106f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c106f-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="c106f-112">Analytics.Read</span></span> |
| <span data-ttu-id="c106f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c106f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c106f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c106f-114">Not supported.</span></span> |
| <span data-ttu-id="c106f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c106f-115">Application</span></span>                            | <span data-ttu-id="c106f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c106f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c106f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c106f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c106f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c106f-118">Optional query parameters</span></span>

<span data-ttu-id="c106f-119">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c106f-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c106f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c106f-120">Request headers</span></span>

| <span data-ttu-id="c106f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c106f-121">Name</span></span>      |<span data-ttu-id="c106f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c106f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c106f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c106f-123">Authorization</span></span> | <span data-ttu-id="c106f-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c106f-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c106f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c106f-125">Request body</span></span>

<span data-ttu-id="c106f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c106f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c106f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c106f-127">Response</span></span>

<span data-ttu-id="c106f-128">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos activityStatistics](../resources/activitystatistics.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c106f-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c106f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c106f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c106f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c106f-130">Request</span></span>

<span data-ttu-id="c106f-131">A seguir está um exemplo de uma solicitação de todas as estatísticas de atividade relacionadas para o usuário in-loco.</span><span class="sxs-lookup"><span data-stu-id="c106f-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="c106f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c106f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="c106f-133">C#</span><span class="sxs-lookup"><span data-stu-id="c106f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c106f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c106f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c106f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c106f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c106f-136">Java</span><span class="sxs-lookup"><span data-stu-id="c106f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitystatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c106f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c106f-137">Response</span></span>

<span data-ttu-id="c106f-138">A seguir está um exemplo de uma resposta com todas as estatísticas de atividade relacionadas para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c106f-138">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="c106f-139">Essa resposta mostra apenas o primeiro dia das atividades de uma semana para reduzi-la para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="c106f-139">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="c106f-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c106f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


