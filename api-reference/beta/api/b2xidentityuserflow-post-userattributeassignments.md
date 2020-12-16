---
title: Criar userAttributeAssignments
description: Criar um novo objeto identityUserFlowAttributeAssignment em um b2xIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a330e365cdb5c198136ae52d3edc3ba197b8c47
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689497"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="68a0c-103">Criar userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="68a0c-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="68a0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68a0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68a0c-105">Criar um novo objeto identityUserFlowAttributeAssignment em um [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="68a0c-105">Create a new identityUserFlowAttributeAssignment object in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68a0c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="68a0c-106">Permissions</span></span>

<span data-ttu-id="68a0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a0c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68a0c-109">Permission type</span></span>|<span data-ttu-id="68a0c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68a0c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68a0c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68a0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68a0c-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a0c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="68a0c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68a0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68a0c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="68a0c-114">Not supported</span></span>|
|<span data-ttu-id="68a0c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68a0c-115">Application</span></span>|<span data-ttu-id="68a0c-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a0c-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68a0c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a0c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="68a0c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68a0c-118">Request headers</span></span>

|<span data-ttu-id="68a0c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="68a0c-119">Name</span></span>|<span data-ttu-id="68a0c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a0c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68a0c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68a0c-121">Authorization</span></span>|<span data-ttu-id="68a0c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a0c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68a0c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68a0c-124">Content-Type</span></span>|<span data-ttu-id="68a0c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a0c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68a0c-127">Request body</span></span>

<span data-ttu-id="68a0c-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="68a0c-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="68a0c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68a0c-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="68a0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68a0c-130">Property</span></span>|<span data-ttu-id="68a0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="68a0c-131">Type</span></span>|<span data-ttu-id="68a0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a0c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="68a0c-133">displayName</span></span>|<span data-ttu-id="68a0c-134">String</span><span class="sxs-lookup"><span data-stu-id="68a0c-134">String</span></span>|<span data-ttu-id="68a0c-135">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="68a0c-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="68a0c-136">IsOptional</span><span class="sxs-lookup"><span data-stu-id="68a0c-136">isOptional</span></span>|<span data-ttu-id="68a0c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="68a0c-137">Boolean</span></span>|<span data-ttu-id="68a0c-138">Determina se o identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="68a0c-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="68a0c-139">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="68a0c-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="68a0c-140">`false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="68a0c-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="68a0c-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="68a0c-141">requiresVerification</span></span>|<span data-ttu-id="68a0c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="68a0c-142">Boolean</span></span>|<span data-ttu-id="68a0c-143">Determina se o identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="68a0c-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="68a0c-144">Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="68a0c-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="68a0c-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="68a0c-145">userAttributeValues</span></span>|<span data-ttu-id="68a0c-146">coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="68a0c-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="68a0c-147">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="68a0c-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="68a0c-148">Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="68a0c-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="68a0c-149">userinputtype</span><span class="sxs-lookup"><span data-stu-id="68a0c-149">userInputType</span></span>|<span data-ttu-id="68a0c-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="68a0c-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="68a0c-151">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="68a0c-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="68a0c-152">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="68a0c-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="68a0c-153">userattribute</span><span class="sxs-lookup"><span data-stu-id="68a0c-153">userAttribute</span></span>|[<span data-ttu-id="68a0c-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="68a0c-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="68a0c-155">O identificador do atributo de fluxo do usuário a ser incluído na atribuição de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="68a0c-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="68a0c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a0c-156">Response</span></span>

<span data-ttu-id="68a0c-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a0c-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68a0c-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68a0c-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68a0c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68a0c-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="68a0c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="68a0c-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="68a0c-161">C#</span><span class="sxs-lookup"><span data-stu-id="68a0c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68a0c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68a0c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68a0c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68a0c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68a0c-164">Java</span><span class="sxs-lookup"><span data-stu-id="68a0c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68a0c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a0c-165">Response</span></span>

<span data-ttu-id="68a0c-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="68a0c-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
