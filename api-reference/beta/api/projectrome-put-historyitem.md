---
title: Criar ou substituir um historyItem
description: Criar uma nova ou substituir um item de histórico existente para uma atividade do usuário existente.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ea4a45f2b9d0021bb339e8edadd9006042a9456
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929694"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="c3295-103">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="c3295-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="c3295-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3295-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3295-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3295-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3295-106">Criar uma nova ou substituir um item de histórico existente para uma atividade do usuário existente.</span><span class="sxs-lookup"><span data-stu-id="c3295-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3295-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3295-107">Permissions</span></span>

<span data-ttu-id="c3295-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3295-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3295-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3295-110">Permission type</span></span>      | <span data-ttu-id="c3295-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3295-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3295-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3295-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3295-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c3295-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c3295-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3295-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3295-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c3295-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c3295-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3295-116">Application</span></span> | <span data-ttu-id="c3295-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3295-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3295-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3295-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="c3295-119">ID deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="c3295-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3295-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3295-120">Request headers</span></span>

|<span data-ttu-id="c3295-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c3295-121">Name</span></span> | <span data-ttu-id="c3295-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3295-122">Type</span></span> | <span data-ttu-id="c3295-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3295-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c3295-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3295-124">Authorization</span></span> | <span data-ttu-id="c3295-125">string</span><span class="sxs-lookup"><span data-stu-id="c3295-125">string</span></span> | <span data-ttu-id="c3295-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3295-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3295-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3295-128">Request body</span></span>

<span data-ttu-id="c3295-129">No corpo da solicitação, fornece uma representação JSON de um objeto [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c3295-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c3295-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3295-130">Response</span></span>

<span data-ttu-id="c3295-131">Se tiver êxito, este método retornará o `201 Created` código de resposta se o historyItem foi criado ou `200 OK` se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="c3295-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="c3295-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3295-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3295-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3295-133">Request</span></span>

<span data-ttu-id="c3295-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3295-134">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c3295-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3295-135">Response</span></span>

<span data-ttu-id="c3295-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3295-136">Here is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
