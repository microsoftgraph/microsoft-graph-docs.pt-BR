---
title: Criar ou substituir um historyItem
description: Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: c1ba6a574f106fd095da4c16ecc5a9826a1ec90d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809926"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="7e337-103">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="7e337-103">Create or replace a historyItem</span></span>

<span data-ttu-id="7e337-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e337-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e337-105">Criar uma nova ou substituir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="7e337-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e337-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e337-106">Permissions</span></span>

<span data-ttu-id="7e337-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e337-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e337-109">Permission type</span></span>      | <span data-ttu-id="7e337-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e337-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e337-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e337-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e337-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7e337-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7e337-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e337-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e337-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7e337-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7e337-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e337-115">Application</span></span> | <span data-ttu-id="7e337-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e337-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e337-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e337-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="7e337-118">ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="7e337-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e337-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e337-119">Request headers</span></span>

|<span data-ttu-id="7e337-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7e337-120">Name</span></span> | <span data-ttu-id="7e337-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e337-121">Type</span></span> | <span data-ttu-id="7e337-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e337-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7e337-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e337-123">Authorization</span></span> | <span data-ttu-id="7e337-124">string</span><span class="sxs-lookup"><span data-stu-id="7e337-124">string</span></span> | <span data-ttu-id="7e337-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e337-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e337-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e337-127">Request body</span></span>

<span data-ttu-id="7e337-128">No corpo da solicitação, forneça uma representação JSON de um objeto [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7e337-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e337-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e337-129">Response</span></span>

<span data-ttu-id="7e337-130">Se tiver êxito, este método retornará o `201 Created` código de resposta se o historyItem foi criado ou `200 OK` se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="7e337-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="7e337-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e337-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e337-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e337-132">Request</span></span>

<span data-ttu-id="7e337-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e337-133">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="7e337-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e337-134">Response</span></span>

<span data-ttu-id="7e337-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e337-135">Here is an example of the response.</span></span>

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
