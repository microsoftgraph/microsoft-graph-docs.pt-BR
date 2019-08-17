---
title: Listar activityStatistics
description: Obtenha uma coleção de objetos activityStatistics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 683dacd86088b2d306abbc36a15e890edbdc1ae6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450687"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="c1229-103">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="c1229-103">List activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1229-104">Obtenha uma coleção de [activityStatistics](../resources/activitystatistics.md) para um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="c1229-104">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1229-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1229-105">Permissions</span></span>

<span data-ttu-id="c1229-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1229-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1229-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1229-108">Permission type</span></span>                        | <span data-ttu-id="c1229-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1229-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1229-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1229-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1229-111">Analytics. Read</span><span class="sxs-lookup"><span data-stu-id="c1229-111">Analytics.Read</span></span> |
| <span data-ttu-id="c1229-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1229-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1229-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1229-113">Not supported.</span></span> |
| <span data-ttu-id="c1229-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1229-114">Application</span></span>                            | <span data-ttu-id="c1229-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1229-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1229-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1229-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET  https://graph.microsoft.com/beta/me/analytics/activitystatistics 
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1229-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1229-117">Optional query parameters</span></span>

<span data-ttu-id="c1229-118">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1229-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1229-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1229-119">Request headers</span></span>

| <span data-ttu-id="c1229-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c1229-120">Name</span></span>      |<span data-ttu-id="c1229-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1229-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1229-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1229-122">Authorization</span></span> | <span data-ttu-id="c1229-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c1229-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1229-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1229-124">Request body</span></span>

<span data-ttu-id="c1229-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1229-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1229-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1229-126">Response</span></span>

<span data-ttu-id="c1229-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [activityStatistics](../resources/activitystatistics.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1229-127">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1229-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1229-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1229-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1229-129">Request</span></span>

<span data-ttu-id="c1229-130">Veja a seguir um exemplo de uma solicitação de todas as estatísticas de atividade relacionadas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c1229-130">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```

### <a name="response"></a><span data-ttu-id="c1229-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1229-131">Response</span></span>

<span data-ttu-id="c1229-132">Veja a seguir um exemplo de uma resposta com todas as estatísticas de atividade relacionadas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c1229-132">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="c1229-133">Essa resposta mostra apenas o primeiro dia das atividades de uma semana para reduzir a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1229-133">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="c1229-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1229-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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