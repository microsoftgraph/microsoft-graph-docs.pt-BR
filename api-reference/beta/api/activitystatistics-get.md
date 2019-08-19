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
# <a name="get-activitystatistics"></a><span data-ttu-id="4f66a-103">Obter activityStatistics</span><span class="sxs-lookup"><span data-stu-id="4f66a-103">Get activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f66a-104">Obter as propriedades de um objeto [activityStatistics](../resources/activitystatistics.md) para um usuário.</span><span class="sxs-lookup"><span data-stu-id="4f66a-104">Get the properties of an [activityStatistics](../resources/activitystatistics.md) object for a user.</span></span>

<span data-ttu-id="4f66a-105">Você pode obter as propriedades de um tipo de [activityStatistics](../resources/activitystatistics.md) para o usuário especificado e o intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="4f66a-105">You can get the properties of a type of [activityStatistics](../resources/activitystatistics.md) for the specified user and date range.</span></span> <span data-ttu-id="4f66a-106">Você pode especificar o tipo de estatísticas e o intervalo de datas usando o formato com suporte da [Propriedade Activity ID](../resources/activitystatistics.md#activity-id-property) para `id` na consulta.</span><span class="sxs-lookup"><span data-stu-id="4f66a-106">You can specify the type of statistics and date range by using the supported format of the [activity id property](../resources/activitystatistics.md#activity-id-property) for `id` in the query.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f66a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f66a-107">Permissions</span></span>

<span data-ttu-id="4f66a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f66a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f66a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f66a-110">Permission type</span></span>                        | <span data-ttu-id="4f66a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f66a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f66a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f66a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f66a-113">Analytics. Read</span><span class="sxs-lookup"><span data-stu-id="4f66a-113">Analytics.Read</span></span> |
| <span data-ttu-id="4f66a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f66a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f66a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f66a-115">Not supported.</span></span> |
| <span data-ttu-id="4f66a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f66a-116">Application</span></span>                            | <span data-ttu-id="4f66a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f66a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f66a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f66a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f66a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f66a-119">Optional query parameters</span></span>

<span data-ttu-id="4f66a-120">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f66a-120">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f66a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f66a-121">Request headers</span></span>

| <span data-ttu-id="4f66a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4f66a-122">Name</span></span>      |<span data-ttu-id="4f66a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f66a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f66a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f66a-124">Authorization</span></span> | <span data-ttu-id="4f66a-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4f66a-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f66a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f66a-126">Request body</span></span>

<span data-ttu-id="4f66a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f66a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f66a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f66a-128">Response</span></span>

<span data-ttu-id="4f66a-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o tipo solicitado de estatísticas de atividade, que é um dos seguintes recursos derivados de [ActivityStatistics](../resources/activitystatistics.md): {[Call](../resources/callactivitystatistics.md), [chat](../resources/chatactivitystatistics.md), [email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), e [reunião](../resources/meetingactivitystatistics.md)}.</span><span class="sxs-lookup"><span data-stu-id="4f66a-129">If successful, this method returns a `200 OK` response code and the requested type of activity statistics, which is one of the following resources derived from [activityStatistics](../resources/activitystatistics.md):{[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), and [Meeting](../resources/meetingactivitystatistics.md)}.</span></span>

## <a name="example"></a><span data-ttu-id="4f66a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f66a-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f66a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f66a-131">Request</span></span>

<span data-ttu-id="4f66a-132">O exemplo a seguir solicita estatísticas do tipo emailActivityStatistics do usuário conectado, para o intervalo de datas entre 2019-06-16 e 2019-06-17.</span><span class="sxs-lookup"><span data-stu-id="4f66a-132">The following example requests statistics of the type emailActivityStatistics of the signed-in user, for the date range between 2019-06-16 and 2019-06-17.</span></span> <span data-ttu-id="4f66a-133">Para obter mais informações sobre o formato de propriedade de ID geral, consulte [Activity ID Property](../resources/activitystatistics.md#activity-id-property).</span><span class="sxs-lookup"><span data-stu-id="4f66a-133">For more information about the general id property format, see [activity id property](../resources/activitystatistics.md#activity-id-property).</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f66a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f66a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f66a-135">C#</span><span class="sxs-lookup"><span data-stu-id="4f66a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f66a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f66a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f66a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4f66a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4f66a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f66a-138">Response</span></span>

<span data-ttu-id="4f66a-139">Veja a seguir um exemplo da resposta que obtém as estatísticas de atividade de um usuário conectado para uma atividade e um dia específicos.</span><span class="sxs-lookup"><span data-stu-id="4f66a-139">The following is an example of the response that gets activity statistics of a signed-in user for a specific activity and day.</span></span>

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
