---
title: Atualizar identityUserFlowAttributeAssignment
description: Atualiza as propriedades de um objeto userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d179602f93ad3e9e44b527364e8cfb1f212c36b
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689207"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="1b360-103">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1b360-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="1b360-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b360-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b360-105">Atualiza as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="1b360-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b360-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1b360-106">Permissions</span></span>

<span data-ttu-id="1b360-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b360-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b360-109">Permission type</span></span>|<span data-ttu-id="1b360-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b360-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b360-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b360-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b360-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b360-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1b360-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b360-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b360-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1b360-114">Not supported</span></span>|
|<span data-ttu-id="1b360-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b360-115">Application</span></span>|<span data-ttu-id="1b360-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b360-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b360-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b360-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b360-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b360-118">Request headers</span></span>

|<span data-ttu-id="1b360-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1b360-119">Name</span></span>|<span data-ttu-id="1b360-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b360-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b360-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b360-121">Authorization</span></span>|<span data-ttu-id="1b360-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b360-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b360-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b360-124">Content-Type</span></span>|<span data-ttu-id="1b360-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b360-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b360-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b360-127">Request body</span></span>

<span data-ttu-id="1b360-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1b360-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="1b360-129">A tabela a seguir mostra as propriedades que estão disponíveis para atualização no [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1b360-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="1b360-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b360-130">Property</span></span>|<span data-ttu-id="1b360-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b360-131">Type</span></span>|<span data-ttu-id="1b360-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b360-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b360-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1b360-133">displayName</span></span>|<span data-ttu-id="1b360-134">String</span><span class="sxs-lookup"><span data-stu-id="1b360-134">String</span></span>|<span data-ttu-id="1b360-135">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="1b360-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="1b360-136">IsOptional</span><span class="sxs-lookup"><span data-stu-id="1b360-136">isOptional</span></span>|<span data-ttu-id="1b360-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b360-137">Boolean</span></span>|<span data-ttu-id="1b360-138">Determina se o identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="1b360-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="1b360-139">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="1b360-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="1b360-140">`false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="1b360-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="1b360-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="1b360-141">requiresVerification</span></span>|<span data-ttu-id="1b360-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b360-142">Boolean</span></span>|<span data-ttu-id="1b360-143">Determina se o identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="1b360-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="1b360-144">Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1b360-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="1b360-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="1b360-145">userAttributeValues</span></span>|<span data-ttu-id="1b360-146">coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b360-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="1b360-147">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1b360-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="1b360-148">Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="1b360-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="1b360-149">userinputtype</span><span class="sxs-lookup"><span data-stu-id="1b360-149">userInputType</span></span>|<span data-ttu-id="1b360-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="1b360-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="1b360-151">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1b360-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="1b360-152">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="1b360-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="1b360-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b360-153">Response</span></span>

<span data-ttu-id="1b360-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b360-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b360-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b360-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b360-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b360-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1b360-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b360-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```
# <a name="c"></a>[<span data-ttu-id="1b360-158">C#</span><span class="sxs-lookup"><span data-stu-id="1b360-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userattributeassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b360-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b360-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userattributeassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b360-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b360-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userattributeassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b360-161">Java</span><span class="sxs-lookup"><span data-stu-id="1b360-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userattributeassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b360-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b360-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
