---
title: Atualizar identityUserFlowAttributeAssignment
description: Atualiza as propriedades de um objeto userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9b5e39cd8d7462b678608ae74727eacdf101cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581294"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="c3458-103">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="c3458-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="c3458-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c3458-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3458-105">Atualiza as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="c3458-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3458-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c3458-106">Permissions</span></span>

<span data-ttu-id="c3458-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3458-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3458-109">Permission type</span></span>|<span data-ttu-id="c3458-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3458-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3458-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3458-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3458-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3458-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c3458-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3458-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3458-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c3458-114">Not supported</span></span>|
|<span data-ttu-id="c3458-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3458-115">Application</span></span>|<span data-ttu-id="c3458-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3458-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3458-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3458-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c3458-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3458-118">Request headers</span></span>

|<span data-ttu-id="c3458-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3458-119">Name</span></span>|<span data-ttu-id="c3458-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3458-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3458-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3458-121">Authorization</span></span>|<span data-ttu-id="c3458-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3458-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3458-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3458-124">Content-Type</span></span>|<span data-ttu-id="c3458-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3458-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3458-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3458-127">Request body</span></span>

<span data-ttu-id="c3458-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c3458-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="c3458-129">A tabela a seguir mostra as propriedades que estão disponíveis para atualização no [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3458-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="c3458-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3458-130">Property</span></span>|<span data-ttu-id="c3458-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3458-131">Type</span></span>|<span data-ttu-id="c3458-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3458-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3458-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c3458-133">displayName</span></span>|<span data-ttu-id="c3458-134">String</span><span class="sxs-lookup"><span data-stu-id="c3458-134">String</span></span>|<span data-ttu-id="c3458-135">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="c3458-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="c3458-136">IsOptional</span><span class="sxs-lookup"><span data-stu-id="c3458-136">isOptional</span></span>|<span data-ttu-id="c3458-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3458-137">Boolean</span></span>|<span data-ttu-id="c3458-138">Determina se o identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="c3458-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="c3458-139">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="c3458-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="c3458-140">`false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="c3458-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="c3458-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="c3458-141">requiresVerification</span></span>|<span data-ttu-id="c3458-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3458-142">Boolean</span></span>|<span data-ttu-id="c3458-143">Determina se o identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="c3458-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="c3458-144">Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3458-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="c3458-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="c3458-145">userAttributeValues</span></span>|<span data-ttu-id="c3458-146">coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="c3458-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="c3458-147">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3458-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="c3458-148">Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="c3458-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="c3458-149">userinputtype</span><span class="sxs-lookup"><span data-stu-id="c3458-149">userInputType</span></span>|<span data-ttu-id="c3458-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="c3458-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="c3458-151">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3458-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="c3458-152">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="c3458-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="c3458-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3458-153">Response</span></span>

<span data-ttu-id="c3458-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3458-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3458-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3458-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3458-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3458-156">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="c3458-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3458-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
