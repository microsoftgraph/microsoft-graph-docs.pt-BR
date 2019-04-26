---
title: Criar ou substituir um historyItem
description: Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 0a8d03029350ce96e7442473dffa0595278bc195
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337249"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="57564-103">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="57564-103">Create or replace a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57564-104">Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="57564-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="57564-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="57564-105">Permissions</span></span>

<span data-ttu-id="57564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57564-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57564-108">Permission type</span></span>      | <span data-ttu-id="57564-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57564-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57564-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57564-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57564-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="57564-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="57564-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57564-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57564-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="57564-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="57564-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57564-114">Application</span></span> | <span data-ttu-id="57564-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57564-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57564-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57564-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="57564-117">ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="57564-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57564-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57564-118">Request headers</span></span>

|<span data-ttu-id="57564-119">Nome</span><span class="sxs-lookup"><span data-stu-id="57564-119">Name</span></span> | <span data-ttu-id="57564-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="57564-120">Type</span></span> | <span data-ttu-id="57564-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="57564-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="57564-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57564-122">Authorization</span></span> | <span data-ttu-id="57564-123">string</span><span class="sxs-lookup"><span data-stu-id="57564-123">string</span></span> | <span data-ttu-id="57564-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57564-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57564-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57564-126">Request body</span></span>

<span data-ttu-id="57564-127">No corpo da solicitação, forneça uma representação JSON de um objeto [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="57564-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57564-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57564-128">Response</span></span>

<span data-ttu-id="57564-129">Se tiver êxito, este método retornará `201 Created` o código de resposta se o historyItem foi `200 OK` criado ou se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="57564-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="57564-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57564-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="57564-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57564-131">Request</span></span>

<span data-ttu-id="57564-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57564-132">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="57564-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="57564-133">Response</span></span>

<span data-ttu-id="57564-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57564-134">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.historyItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
