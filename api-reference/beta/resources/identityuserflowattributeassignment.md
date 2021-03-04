---
title: tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usados para coletar identidade específicaUserFlowAttributes em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0b1b0addc48b96eeb3f19c9acf2a8b01e8891efb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440224"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="1a849-103">tipo de recurso identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1a849-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="1a849-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a849-105">identityUserFlowAttributeAssignments são usados para coletar identidade específicaUserFlowAttributes em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="1a849-106">Isso permite o controle sobre os atributos coletados em um fluxo de usuários e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="1a849-107">Você pode ter várias identidadesUserFlowAttributeAssignments em um único fluxo de usuários que cria a experiência que o usuário final vê durante a assinatura quando solicitado a fornecer as informações necessárias pelo fluxo do usuário para concluir a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1a849-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="1a849-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1a849-108">Methods</span></span>

|<span data-ttu-id="1a849-109">Método</span><span class="sxs-lookup"><span data-stu-id="1a849-109">Method</span></span>|<span data-ttu-id="1a849-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a849-110">Return type</span></span>|<span data-ttu-id="1a849-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a849-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a849-112">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1a849-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="1a849-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1a849-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="1a849-114">Leia as propriedades e as relações de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="1a849-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="1a849-115">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1a849-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="1a849-116">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="1a849-116">None</span></span>|<span data-ttu-id="1a849-117">Atualize as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="1a849-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="1a849-118">Excluir identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1a849-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="1a849-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="1a849-119">None</span></span>|<span data-ttu-id="1a849-120">Exclua um objeto identityUserFlowAttributeAssignment específico.</span><span class="sxs-lookup"><span data-stu-id="1a849-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="1a849-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="1a849-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="1a849-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="1a849-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="1a849-123">Obtém a ordem da identityUserFlowAttributes sendo coletada dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="1a849-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="1a849-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="1a849-125">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="1a849-125">None</span></span>|<span data-ttu-id="1a849-126">Define a ordem da identidadeUserFlowAttributes sendo coletada dentro de um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="1a849-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a849-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a849-127">Properties</span></span>

|<span data-ttu-id="1a849-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a849-128">Property</span></span>|<span data-ttu-id="1a849-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a849-129">Type</span></span>|<span data-ttu-id="1a849-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a849-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a849-131">id</span><span class="sxs-lookup"><span data-stu-id="1a849-131">id</span></span>|<span data-ttu-id="1a849-132">String</span><span class="sxs-lookup"><span data-stu-id="1a849-132">String</span></span>|<span data-ttu-id="1a849-133">O identificador da identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="1a849-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="1a849-134">Esse identificador é imutável depois de criado.</span><span class="sxs-lookup"><span data-stu-id="1a849-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="1a849-135">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a849-135">This is a read-only property.</span></span>|
|<span data-ttu-id="1a849-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1a849-136">displayName</span></span>|<span data-ttu-id="1a849-137">String</span><span class="sxs-lookup"><span data-stu-id="1a849-137">String</span></span>|<span data-ttu-id="1a849-138">O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="1a849-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="1a849-139">isOptional</span></span>|<span data-ttu-id="1a849-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a849-140">Boolean</span></span>|<span data-ttu-id="1a849-141">Determina se identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="1a849-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="1a849-142">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="1a849-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="1a849-143">`false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="1a849-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="1a849-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="1a849-144">requiresVerification</span></span>|<span data-ttu-id="1a849-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a849-145">Boolean</span></span>|<span data-ttu-id="1a849-146">Determina se identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="1a849-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="1a849-147">Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="1a849-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="1a849-148">userAttributeValues</span></span>|<span data-ttu-id="1a849-149">[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a849-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="1a849-150">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="1a849-151">Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="1a849-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="1a849-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="1a849-152">userInputType</span></span>|<span data-ttu-id="1a849-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="1a849-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="1a849-154">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1a849-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="1a849-155">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="1a849-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a849-156">Relações</span><span class="sxs-lookup"><span data-stu-id="1a849-156">Relationships</span></span>

|<span data-ttu-id="1a849-157">Relação</span><span class="sxs-lookup"><span data-stu-id="1a849-157">Relationship</span></span>|<span data-ttu-id="1a849-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a849-158">Type</span></span>|<span data-ttu-id="1a849-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a849-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a849-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="1a849-160">userAttribute</span></span>|[<span data-ttu-id="1a849-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="1a849-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="1a849-162">O atributo do usuário que você deseja adicionar ao seu fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="1a849-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a849-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a849-163">JSON representation</span></span>

<span data-ttu-id="1a849-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a849-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
