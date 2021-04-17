---
title: Excluir identityUserFlowAttribute
description: Exclua uma identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: c5289130cb54ca68889cb5875d6277fe73de1e09
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882392"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="fecd5-103">Excluir identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="fecd5-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="fecd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fecd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fecd5-105">Excluir uma [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="fecd5-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="fecd5-106">Somente atributos de fluxo de usuário personalizados podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="fecd5-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="fecd5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fecd5-107">Permissions</span></span>

<span data-ttu-id="fecd5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fecd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fecd5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fecd5-110">Permission type</span></span>      | <span data-ttu-id="fecd5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fecd5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fecd5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fecd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fecd5-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecd5-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fecd5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fecd5-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fecd5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fecd5-115">Not supported.</span></span>|
|<span data-ttu-id="fecd5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fecd5-116">Application</span></span>|<span data-ttu-id="fecd5-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecd5-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fecd5-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fecd5-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fecd5-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fecd5-119">Global administrator</span></span>
* <span data-ttu-id="fecd5-120">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fecd5-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fecd5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fecd5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fecd5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fecd5-122">Request headers</span></span>

|<span data-ttu-id="fecd5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fecd5-123">Name</span></span>|<span data-ttu-id="fecd5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fecd5-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fecd5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fecd5-125">Authorization</span></span>|<span data-ttu-id="fecd5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fecd5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fecd5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fecd5-128">Request body</span></span>

<span data-ttu-id="fecd5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fecd5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fecd5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fecd5-130">Response</span></span>

<span data-ttu-id="fecd5-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fecd5-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fecd5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fecd5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fecd5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fecd5-133">Request</span></span>

<span data-ttu-id="fecd5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fecd5-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
```

### <a name="response"></a><span data-ttu-id="fecd5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fecd5-135">Response</span></span>

<span data-ttu-id="fecd5-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fecd5-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
