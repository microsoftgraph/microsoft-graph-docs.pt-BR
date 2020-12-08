---
title: Criar userAttributeAssignments
description: Criar um novo objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c838dfee57e264d7cca61ac5e10ec98a46f7330
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581279"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="37d7e-103">Criar userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="37d7e-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="37d7e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37d7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37d7e-105">Criar um novo objeto identityUserFlowAttributeAssignment em um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="37d7e-105">Create a new identityUserFlowAttributeAssignment object in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37d7e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="37d7e-106">Permissions</span></span>

<span data-ttu-id="37d7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d7e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37d7e-109">Permission type</span></span>|<span data-ttu-id="37d7e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37d7e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d7e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37d7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37d7e-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="37d7e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="37d7e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37d7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d7e-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="37d7e-114">Not supported</span></span>|
|<span data-ttu-id="37d7e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37d7e-115">Application</span></span>|<span data-ttu-id="37d7e-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="37d7e-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d7e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37d7e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="37d7e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37d7e-118">Request headers</span></span>

|<span data-ttu-id="37d7e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37d7e-119">Name</span></span>|<span data-ttu-id="37d7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d7e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37d7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37d7e-121">Authorization</span></span>|<span data-ttu-id="37d7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37d7e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="37d7e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37d7e-124">Content-Type</span></span>|<span data-ttu-id="37d7e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37d7e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d7e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37d7e-127">Request body</span></span>

<span data-ttu-id="37d7e-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="37d7e-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="37d7e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37d7e-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="37d7e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37d7e-130">Property</span></span>|<span data-ttu-id="37d7e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37d7e-131">Type</span></span>|<span data-ttu-id="37d7e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d7e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="37d7e-133">displayName</span></span>|<span data-ttu-id="37d7e-134">String</span><span class="sxs-lookup"><span data-stu-id="37d7e-134">String</span></span>|<span data-ttu-id="37d7e-135">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="37d7e-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="37d7e-136">IsOptional</span><span class="sxs-lookup"><span data-stu-id="37d7e-136">isOptional</span></span>|<span data-ttu-id="37d7e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d7e-137">Boolean</span></span>|<span data-ttu-id="37d7e-138">Determina se o identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="37d7e-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="37d7e-139">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="37d7e-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="37d7e-140">`false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="37d7e-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="37d7e-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="37d7e-141">requiresVerification</span></span>|<span data-ttu-id="37d7e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d7e-142">Boolean</span></span>|<span data-ttu-id="37d7e-143">Determina se o identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="37d7e-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="37d7e-144">Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="37d7e-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="37d7e-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="37d7e-145">userAttributeValues</span></span>|<span data-ttu-id="37d7e-146">coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="37d7e-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="37d7e-147">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="37d7e-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="37d7e-148">Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="37d7e-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="37d7e-149">userinputtype</span><span class="sxs-lookup"><span data-stu-id="37d7e-149">userInputType</span></span>|<span data-ttu-id="37d7e-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="37d7e-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="37d7e-151">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="37d7e-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="37d7e-152">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="37d7e-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="37d7e-153">userattribute</span><span class="sxs-lookup"><span data-stu-id="37d7e-153">userAttribute</span></span>|[<span data-ttu-id="37d7e-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="37d7e-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="37d7e-155">O identificador do atributo de fluxo do usuário a ser incluído na atribuição de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="37d7e-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="37d7e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d7e-156">Response</span></span>

<span data-ttu-id="37d7e-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37d7e-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37d7e-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37d7e-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37d7e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37d7e-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments
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

### <a name="response"></a><span data-ttu-id="37d7e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d7e-160">Response</span></span>

<span data-ttu-id="37d7e-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37d7e-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2C_1_Consumer/userAttributeAssignments/extension_guid_shoeSize
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
