---
title: Atualizar identityUserFlowAttributeAssignment
description: Atualize as propriedades de um objeto userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 42ca1bd9d646e99fb254ad01c0c00512fbba441e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882784"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="f5065-103">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="f5065-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="f5065-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5065-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5065-105">Atualize as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="f5065-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5065-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5065-106">Permissions</span></span>

<span data-ttu-id="f5065-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5065-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5065-109">Permission type</span></span>|<span data-ttu-id="f5065-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5065-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5065-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5065-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5065-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5065-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f5065-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5065-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5065-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f5065-114">Not supported</span></span>|
|<span data-ttu-id="f5065-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5065-115">Application</span></span>|<span data-ttu-id="f5065-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5065-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5065-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5065-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5065-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5065-118">Request headers</span></span>

|<span data-ttu-id="f5065-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f5065-119">Name</span></span>|<span data-ttu-id="f5065-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5065-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5065-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5065-121">Authorization</span></span>|<span data-ttu-id="f5065-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5065-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f5065-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5065-124">Content-Type</span></span>|<span data-ttu-id="f5065-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5065-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5065-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5065-127">Request body</span></span>

<span data-ttu-id="f5065-128">No corpo da solicitação, fornece uma representação JSON do [objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f5065-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="f5065-129">A tabela a seguir mostra as propriedades disponíveis para atualização na [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f5065-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="f5065-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5065-130">Property</span></span>|<span data-ttu-id="f5065-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5065-131">Type</span></span>|<span data-ttu-id="f5065-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5065-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5065-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f5065-133">displayName</span></span>|<span data-ttu-id="f5065-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5065-134">String</span></span>|<span data-ttu-id="f5065-135">O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="f5065-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="f5065-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="f5065-136">isOptional</span></span>|<span data-ttu-id="f5065-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5065-137">Boolean</span></span>|<span data-ttu-id="f5065-138">Determina se identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="f5065-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="f5065-139">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="f5065-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="f5065-140">`false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="f5065-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="f5065-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="f5065-141">requiresVerification</span></span>|<span data-ttu-id="f5065-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5065-142">Boolean</span></span>|<span data-ttu-id="f5065-143">Determina se identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="f5065-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="f5065-144">Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f5065-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="f5065-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="f5065-145">userAttributeValues</span></span>|<span data-ttu-id="f5065-146">[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5065-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="f5065-147">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f5065-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="f5065-148">Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="f5065-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="f5065-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="f5065-149">userInputType</span></span>|<span data-ttu-id="f5065-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="f5065-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="f5065-151">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f5065-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="f5065-152">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="f5065-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="f5065-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5065-153">Response</span></span>

<span data-ttu-id="f5065-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5065-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5065-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5065-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5065-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5065-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a><span data-ttu-id="f5065-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5065-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
