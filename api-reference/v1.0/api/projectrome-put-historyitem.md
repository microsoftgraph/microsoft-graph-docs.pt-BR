---
title: Criar ou substituir um historyItem
description: Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: ce1abf2ea6df1e7a289802073a47bd1b9fdeb005
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510701"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="273e9-103">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="273e9-103">Create or replace a historyItem</span></span>

<span data-ttu-id="273e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="273e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="273e9-105">Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="273e9-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="273e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="273e9-106">Permissions</span></span>

<span data-ttu-id="273e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="273e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="273e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="273e9-109">Permission type</span></span>      | <span data-ttu-id="273e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="273e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="273e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="273e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="273e9-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="273e9-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="273e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="273e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="273e9-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="273e9-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="273e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="273e9-115">Application</span></span> | <span data-ttu-id="273e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="273e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="273e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="273e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="273e9-118">ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="273e9-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="273e9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="273e9-119">Request headers</span></span>

|<span data-ttu-id="273e9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="273e9-120">Name</span></span> | <span data-ttu-id="273e9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="273e9-121">Type</span></span> | <span data-ttu-id="273e9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="273e9-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="273e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="273e9-123">Authorization</span></span> | <span data-ttu-id="273e9-124">string</span><span class="sxs-lookup"><span data-stu-id="273e9-124">string</span></span> | <span data-ttu-id="273e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="273e9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="273e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="273e9-127">Request body</span></span>

<span data-ttu-id="273e9-128">No corpo da solicitação, forneça uma representação JSON de um objeto [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="273e9-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="273e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="273e9-129">Response</span></span>

<span data-ttu-id="273e9-130">Se tiver êxito, este método retornará `201 Created` o código de resposta se o historyItem foi `200 OK` criado ou se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="273e9-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="273e9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="273e9-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="273e9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="273e9-132">Request</span></span>

<span data-ttu-id="273e9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="273e9-133">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="273e9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="273e9-134">Response</span></span>

<span data-ttu-id="273e9-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="273e9-135">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
