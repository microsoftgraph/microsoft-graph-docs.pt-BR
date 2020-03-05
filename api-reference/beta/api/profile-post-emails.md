---
title: Criar email
description: Criar um novo email.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c273e7c826d8222596521948c91f48d939657575
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455106"
---
# <a name="create-itememail"></a><span data-ttu-id="2ee86-103">Criar email</span><span class="sxs-lookup"><span data-stu-id="2ee86-103">Create itemEmail</span></span>

<span data-ttu-id="2ee86-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ee86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee86-105">Criar um novo [email](../resources/itememail.md).</span><span class="sxs-lookup"><span data-stu-id="2ee86-105">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ee86-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ee86-106">Permissions</span></span>

<span data-ttu-id="2ee86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ee86-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ee86-109">Permission type</span></span>                        | <span data-ttu-id="2ee86-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ee86-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ee86-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ee86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ee86-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2ee86-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2ee86-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ee86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ee86-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2ee86-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2ee86-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ee86-115">Application</span></span>                            | <span data-ttu-id="2ee86-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee86-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ee86-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="2ee86-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee86-118">Request headers</span></span>

| <span data-ttu-id="2ee86-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ee86-119">Name</span></span>      |<span data-ttu-id="2ee86-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee86-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ee86-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ee86-121">Authorization</span></span>  | <span data-ttu-id="2ee86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee86-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2ee86-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ee86-124">Content-Type</span></span>   | <span data-ttu-id="2ee86-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee86-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ee86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee86-127">Request body</span></span>

<span data-ttu-id="2ee86-128">No corpo da solicitação, forneça uma representação JSON de um objeto de [email](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="2ee86-128">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ee86-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee86-129">Response</span></span>

<span data-ttu-id="2ee86-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto de [email](../resources/itememail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee86-130">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ee86-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ee86-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ee86-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee86-132">Request</span></span>

<span data-ttu-id="2ee86-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ee86-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/user/profile/emails
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="2ee86-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee86-134">Response</span></span>

<span data-ttu-id="2ee86-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee86-135">The following is an example of the response.</span></span>

> <span data-ttu-id="2ee86-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ee86-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
