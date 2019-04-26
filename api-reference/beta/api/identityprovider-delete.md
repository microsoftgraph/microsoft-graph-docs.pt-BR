---
title: Excluir identityProvider
description: Excluir o identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: 512d7b1094af967c10cb5ddf6eb2c9178d9d8ad7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328525"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="64235-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="64235-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64235-104">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="64235-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64235-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64235-105">Permissions</span></span>

<span data-ttu-id="64235-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64235-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64235-108">Permission type</span></span>      | <span data-ttu-id="64235-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64235-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64235-110">Delegated (work or school account)</span></span>|<span data-ttu-id="64235-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64235-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="64235-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64235-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="64235-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64235-113">Not supported.</span></span>|
|<span data-ttu-id="64235-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64235-114">Application</span></span>|<span data-ttu-id="64235-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64235-115">Not supported.</span></span>|

<span data-ttu-id="64235-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="64235-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="64235-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64235-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="64235-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64235-118">Request headers</span></span>

|<span data-ttu-id="64235-119">Nome</span><span class="sxs-lookup"><span data-stu-id="64235-119">Name</span></span>|<span data-ttu-id="64235-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64235-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="64235-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64235-121">Authorization</span></span>|<span data-ttu-id="64235-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64235-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64235-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64235-124">Request body</span></span>

<span data-ttu-id="64235-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64235-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64235-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="64235-126">Response</span></span>

<span data-ttu-id="64235-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64235-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64235-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64235-128">Example</span></span>

<span data-ttu-id="64235-129">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="64235-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="64235-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64235-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="64235-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64235-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
