---
title: Tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usadas para coletar identityUserFlowAttributes específicas em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65859cb0d235454577e236761064f4597f5c68d8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158783"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="0271c-103">Tipo de recurso identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0271c-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="0271c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0271c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0271c-105">identityUserFlowAttributeAssignments são usadas para coletar identityUserFlowAttributes específicas em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="0271c-106">Isso permite o controle sobre os atributos que são coletados em um fluxo de usuário e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="0271c-107">Você pode ter vários identityUserFlowAttributeAssignments dentro de um único fluxo de usuário que cria a experiência que o usuário final vê durante a assinatura quando solicitado a fornecer as informações necessárias pelo fluxo do usuário para concluir a assinatura.</span><span class="sxs-lookup"><span data-stu-id="0271c-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="0271c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0271c-108">Methods</span></span>

|<span data-ttu-id="0271c-109">Método</span><span class="sxs-lookup"><span data-stu-id="0271c-109">Method</span></span>|<span data-ttu-id="0271c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0271c-110">Return type</span></span>|<span data-ttu-id="0271c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0271c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0271c-112">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0271c-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="0271c-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0271c-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="0271c-114">Leia as propriedades e os relacionamentos de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="0271c-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="0271c-115">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0271c-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="0271c-116">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0271c-116">None</span></span>|<span data-ttu-id="0271c-117">Atualizar as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="0271c-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="0271c-118">Excluir identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0271c-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="0271c-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0271c-119">None</span></span>|<span data-ttu-id="0271c-120">Exclua um objeto identityUserFlowAttributeAssignment específico.</span><span class="sxs-lookup"><span data-stu-id="0271c-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="0271c-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="0271c-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="0271c-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="0271c-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="0271c-123">Obtém a ordem dos identityUserFlowAttributes que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="0271c-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="0271c-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="0271c-125">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0271c-125">None</span></span>|<span data-ttu-id="0271c-126">Define a ordem dos identityUserFlowAttributes que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="0271c-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0271c-127">Properties</span></span>

|<span data-ttu-id="0271c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0271c-128">Property</span></span>|<span data-ttu-id="0271c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0271c-129">Type</span></span>|<span data-ttu-id="0271c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0271c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0271c-131">id</span><span class="sxs-lookup"><span data-stu-id="0271c-131">id</span></span>|<span data-ttu-id="0271c-132">String</span><span class="sxs-lookup"><span data-stu-id="0271c-132">String</span></span>|<span data-ttu-id="0271c-133">O identificador do identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="0271c-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="0271c-134">Esse identificador é imutável depois de criado.</span><span class="sxs-lookup"><span data-stu-id="0271c-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="0271c-135">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0271c-135">This is a read-only property.</span></span>|
|<span data-ttu-id="0271c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0271c-136">displayName</span></span>|<span data-ttu-id="0271c-137">String</span><span class="sxs-lookup"><span data-stu-id="0271c-137">String</span></span>|<span data-ttu-id="0271c-138">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="0271c-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="0271c-139">isOptional</span></span>|<span data-ttu-id="0271c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271c-140">Boolean</span></span>|<span data-ttu-id="0271c-141">Determina se a identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="0271c-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="0271c-142">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="0271c-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="0271c-143">`false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="0271c-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="0271c-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="0271c-144">requiresVerification</span></span>|<span data-ttu-id="0271c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271c-145">Boolean</span></span>|<span data-ttu-id="0271c-146">Determina se a identityUserFlowAttribute exige verificação.</span><span class="sxs-lookup"><span data-stu-id="0271c-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="0271c-147">Isso é usado somente para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="0271c-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="0271c-148">userAttributeValues</span></span>|<span data-ttu-id="0271c-149">[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="0271c-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="0271c-150">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="0271c-151">Aplicável somente quando userInputType for `radioSingleSelect` `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="0271c-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="0271c-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="0271c-152">userInputType</span></span>|<span data-ttu-id="0271c-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="0271c-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="0271c-154">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="0271c-155">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="0271c-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0271c-156">Relações</span><span class="sxs-lookup"><span data-stu-id="0271c-156">Relationships</span></span>

|<span data-ttu-id="0271c-157">Relação</span><span class="sxs-lookup"><span data-stu-id="0271c-157">Relationship</span></span>|<span data-ttu-id="0271c-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="0271c-158">Type</span></span>|<span data-ttu-id="0271c-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="0271c-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0271c-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="0271c-160">userAttribute</span></span>|[<span data-ttu-id="0271c-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0271c-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="0271c-162">O atributo de usuário que você deseja adicionar ao seu fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="0271c-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0271c-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0271c-163">JSON representation</span></span>

<span data-ttu-id="0271c-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0271c-164">The following is a JSON representation of the resource.</span></span>
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
