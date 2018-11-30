---
title: Criar ou substituir um historyItem
description: Criar uma nova ou substituir um item de histórico existente para uma atividade do usuário existente.
ms.openlocfilehash: 068e5cb4b98879c1dba5eeef56517b99c3fe47c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040824"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="78535-103">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="78535-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="78535-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78535-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78535-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78535-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78535-106">Criar uma nova ou substituir um item de histórico existente para uma atividade do usuário existente.</span><span class="sxs-lookup"><span data-stu-id="78535-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="78535-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="78535-107">Permissions</span></span>

<span data-ttu-id="78535-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78535-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="78535-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78535-110">Permission type</span></span>      | <span data-ttu-id="78535-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78535-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78535-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78535-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78535-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="78535-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="78535-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78535-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78535-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="78535-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="78535-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78535-116">Application</span></span> | <span data-ttu-id="78535-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78535-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78535-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78535-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="78535-119">ID deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="78535-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78535-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78535-120">Request headers</span></span>

|<span data-ttu-id="78535-121">Nome</span><span class="sxs-lookup"><span data-stu-id="78535-121">Name</span></span> | <span data-ttu-id="78535-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="78535-122">Type</span></span> | <span data-ttu-id="78535-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="78535-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="78535-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="78535-124">Authorization</span></span> | <span data-ttu-id="78535-125">string</span><span class="sxs-lookup"><span data-stu-id="78535-125">string</span></span> | <span data-ttu-id="78535-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78535-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78535-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78535-128">Request body</span></span>

<span data-ttu-id="78535-129">No corpo da solicitação, fornece uma representação JSON de um objeto [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="78535-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78535-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="78535-130">Response</span></span>

<span data-ttu-id="78535-131">Se tiver êxito, este método retornará o `201 Created` código de resposta se o historyItem foi criado ou `200 OK` se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="78535-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="78535-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78535-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="78535-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78535-133">Request</span></span>

<span data-ttu-id="78535-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78535-134">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="78535-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="78535-135">Response</span></span>

<span data-ttu-id="78535-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78535-136">Here is an example of the response.</span></span>

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