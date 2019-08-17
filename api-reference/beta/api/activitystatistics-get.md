---
title: Obter activityStatistics
description: Recupere as propriedades de um objeto activityStatistics para um usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9a85211faf15b6edbf843c5c604251dae06ae0a3
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450688"
---
# <a name="get-activitystatistics"></a><span data-ttu-id="e71f8-103">Obter activityStatistics</span><span class="sxs-lookup"><span data-stu-id="e71f8-103">Get activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71f8-104">Obter as propriedades de um objeto [activityStatistics](../resources/activitystatistics.md) para um usuário.</span><span class="sxs-lookup"><span data-stu-id="e71f8-104">Get the properties of an [activityStatistics](../resources/activitystatistics.md) object for a user.</span></span>

<span data-ttu-id="e71f8-105">Você pode obter as propriedades de um tipo de [activityStatistics](../resources/activitystatistics.md) para o usuário especificado e o intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="e71f8-105">You can get the properties of a type of [activityStatistics](../resources/activitystatistics.md) for the specified user and date range.</span></span> <span data-ttu-id="e71f8-106">Você pode especificar o tipo de estatísticas e o intervalo de datas usando o formato com suporte da [Propriedade Activity ID](../resources/activitystatistics.md#activity-id-property) para `id` na consulta.</span><span class="sxs-lookup"><span data-stu-id="e71f8-106">You can specify the type of statistics and date range by using the supported format of the [activity id property](../resources/activitystatistics.md#activity-id-property) for `id` in the query.</span></span>

## <a name="permissions"></a><span data-ttu-id="e71f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e71f8-107">Permissions</span></span>

<span data-ttu-id="e71f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e71f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e71f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e71f8-110">Permission type</span></span>                        | <span data-ttu-id="e71f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e71f8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e71f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e71f8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e71f8-113">Analytics. Read</span><span class="sxs-lookup"><span data-stu-id="e71f8-113">Analytics.Read</span></span> |
| <span data-ttu-id="e71f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e71f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e71f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e71f8-115">Not supported.</span></span> |
| <span data-ttu-id="e71f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e71f8-116">Application</span></span>                            | <span data-ttu-id="e71f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e71f8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e71f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e71f8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="e71f8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e71f8-119">Optional query parameters</span></span>

<span data-ttu-id="e71f8-120">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e71f8-120">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e71f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e71f8-121">Request headers</span></span>

| <span data-ttu-id="e71f8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e71f8-122">Name</span></span>      |<span data-ttu-id="e71f8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e71f8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e71f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e71f8-124">Authorization</span></span> | <span data-ttu-id="e71f8-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e71f8-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e71f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e71f8-126">Request body</span></span>

<span data-ttu-id="e71f8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e71f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e71f8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71f8-128">Response</span></span>

<span data-ttu-id="e71f8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o tipo solicitado de estatísticas de atividade, que é um dos seguintes recursos derivados de [ActivityStatistics](../resources/activitystatistics.md): {[Call](../resources/callactivitystatistics.md), [chat](../resources/chatactivitystatistics.md), [email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), e [reunião](../resources/meetingactivitystatistics.md)}.</span><span class="sxs-lookup"><span data-stu-id="e71f8-129">If successful, this method returns a `200 OK` response code and the requested type of activity statistics, which is one of the following resources derived from [activityStatistics](../resources/activitystatistics.md):{[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), and [Meeting](../resources/meetingactivitystatistics.md)}.</span></span>

## <a name="example"></a><span data-ttu-id="e71f8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e71f8-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e71f8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e71f8-131">Request</span></span>

<span data-ttu-id="e71f8-132">O exemplo a seguir solicita estatísticas do tipo emailActivityStatistics do usuário conectado, para o intervalo de datas entre 2019-06-16 e 2019-06-17.</span><span class="sxs-lookup"><span data-stu-id="e71f8-132">The following example requests statistics of the type emailActivityStatistics of the signed-in user, for the date range between 2019-06-16 and 2019-06-17.</span></span> <span data-ttu-id="e71f8-133">Para obter mais informações sobre o formato de propriedade de ID geral, consulte [Activity ID Property](../resources/activitystatistics.md#activity-id-property).</span><span class="sxs-lookup"><span data-stu-id="e71f8-133">For more information about the general id property format, see [activity id property](../resources/activitystatistics.md#activity-id-property).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```

#### <a name="response"></a><span data-ttu-id="e71f8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71f8-134">Response</span></span>

<span data-ttu-id="e71f8-135">Veja a seguir um exemplo da resposta que obtém as estatísticas de atividade de um usuário conectado para uma atividade e um dia específicos.</span><span class="sxs-lookup"><span data-stu-id="e71f8-135">The following is an example of the response that gets activity statistics of a signed-in user for a specific activity and day.</span></span>

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
