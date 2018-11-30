---
title: Excluir identityProvider
description: Exclua um identityProvider existente.
ms.openlocfilehash: ac6f8cafa72b94891a540c05c2d4e5e2f32e23c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032974"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="b14f0-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="b14f0-103">Delete identityProvider</span></span>

> <span data-ttu-id="b14f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b14f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b14f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b14f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b14f0-106">Exclua um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b14f0-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b14f0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b14f0-107">Permissions</span></span>

<span data-ttu-id="b14f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b14f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b14f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b14f0-110">Permission type</span></span>      | <span data-ttu-id="b14f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b14f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b14f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b14f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b14f0-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b14f0-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b14f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b14f0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b14f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b14f0-115">Not supported.</span></span>|
|<span data-ttu-id="b14f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b14f0-116">Application</span></span>|<span data-ttu-id="b14f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b14f0-117">Not supported.</span></span>|

<span data-ttu-id="b14f0-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="b14f0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b14f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b14f0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b14f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b14f0-120">Request headers</span></span>

|<span data-ttu-id="b14f0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b14f0-121">Name</span></span>|<span data-ttu-id="b14f0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b14f0-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b14f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b14f0-123">Authorization</span></span>|<span data-ttu-id="b14f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b14f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b14f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b14f0-126">Request body</span></span>

<span data-ttu-id="b14f0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b14f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b14f0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b14f0-128">Response</span></span>

<span data-ttu-id="b14f0-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b14f0-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b14f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b14f0-130">Example</span></span>

<span data-ttu-id="b14f0-131">O exemplo a seguir exclui uma **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="b14f0-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b14f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b14f0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="b14f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b14f0-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->