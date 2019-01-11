---
title: Excluir identityProvider
description: Exclua um identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: 35689037d4f6a564ee3e1e40d18401ef793ef474
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808292"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="57e60-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="57e60-103">Delete identityProvider</span></span>

> <span data-ttu-id="57e60-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="57e60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57e60-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57e60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57e60-106">Exclua um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="57e60-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57e60-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="57e60-107">Permissions</span></span>

<span data-ttu-id="57e60-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57e60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57e60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57e60-110">Permission type</span></span>      | <span data-ttu-id="57e60-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57e60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57e60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57e60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57e60-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e60-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="57e60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57e60-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="57e60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57e60-115">Not supported.</span></span>|
|<span data-ttu-id="57e60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57e60-116">Application</span></span>|<span data-ttu-id="57e60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57e60-117">Not supported.</span></span>|

<span data-ttu-id="57e60-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="57e60-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="57e60-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57e60-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="57e60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57e60-120">Request headers</span></span>

|<span data-ttu-id="57e60-121">Nome</span><span class="sxs-lookup"><span data-stu-id="57e60-121">Name</span></span>|<span data-ttu-id="57e60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="57e60-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="57e60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57e60-123">Authorization</span></span>|<span data-ttu-id="57e60-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57e60-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57e60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57e60-126">Request body</span></span>

<span data-ttu-id="57e60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57e60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57e60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e60-128">Response</span></span>

<span data-ttu-id="57e60-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57e60-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57e60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57e60-130">Example</span></span>

<span data-ttu-id="57e60-131">O exemplo a seguir exclui uma **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="57e60-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="57e60-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57e60-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="57e60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e60-133">Response</span></span>

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
