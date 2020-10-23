---
title: Atualizar identityUserFlowAttribute
description: Atualizar propriedades de um identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe74ffc6b360c2f83b917e9852a42faa6e193955
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742341"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="e4d9c-103">Atualizar identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="e4d9c-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="e4d9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4d9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4d9c-105">Atualiza as propriedades de um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="e4d9c-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="e4d9c-106">Somente atributos de fluxo de usuário personalizados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4d9c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4d9c-107">Permissions</span></span>

<span data-ttu-id="e4d9c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4d9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4d9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4d9c-110">Permission type</span></span>      | <span data-ttu-id="e4d9c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4d9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4d9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4d9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4d9c-113">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e4d9c-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e4d9c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4d9c-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e4d9c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-115">Not supported.</span></span>|
|<span data-ttu-id="e4d9c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4d9c-116">Application</span></span>| <span data-ttu-id="e4d9c-117">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e4d9c-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e4d9c-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e4d9c-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e4d9c-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e4d9c-119">Global administrator</span></span>
* <span data-ttu-id="e4d9c-120">Administrador de atributos de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="e4d9c-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e4d9c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4d9c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e4d9c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d9c-122">Request headers</span></span>

|<span data-ttu-id="e4d9c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e4d9c-123">Name</span></span>|<span data-ttu-id="e4d9c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d9c-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e4d9c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4d9c-125">Authorization</span></span>|<span data-ttu-id="e4d9c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4d9c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4d9c-128">Content-Type</span></span>|<span data-ttu-id="e4d9c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4d9c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d9c-131">Request body</span></span>

<span data-ttu-id="e4d9c-132">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="e4d9c-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="e4d9c-133">**Observação:** Somente a propriedade **Description** pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="e4d9c-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4d9c-134">Property</span></span>|<span data-ttu-id="e4d9c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4d9c-135">Type</span></span>|<span data-ttu-id="e4d9c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d9c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4d9c-137">description</span><span class="sxs-lookup"><span data-stu-id="e4d9c-137">description</span></span>|<span data-ttu-id="e4d9c-138">String</span><span class="sxs-lookup"><span data-stu-id="e4d9c-138">String</span></span>|<span data-ttu-id="e4d9c-139">A descrição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-139">The description of the user flow attribute.</span></span> <span data-ttu-id="e4d9c-140">Ele é exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="e4d9c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4d9c-141">Response</span></span>

<span data-ttu-id="e4d9c-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e4d9c-143">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="e4d9c-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e4d9c-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4d9c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d9c-145">Request</span></span>

<span data-ttu-id="e4d9c-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```

### <a name="response"></a><span data-ttu-id="e4d9c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4d9c-147">Response</span></span>

<span data-ttu-id="e4d9c-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4d9c-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
