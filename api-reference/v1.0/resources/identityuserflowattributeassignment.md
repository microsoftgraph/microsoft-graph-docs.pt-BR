---
title: tipo de recurso identityUserFlowAttributeAssignment
description: Representa como os atributos são coletados em um fluxo de usuário de identidade.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0df6309682158e3d4890c6549bc7aeebb710254c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882782"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="917b4-103">tipo de recurso identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="917b4-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="917b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="917b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="917b4-105">Representa como os atributos são coletados em um fluxo de usuário de identidade.</span><span class="sxs-lookup"><span data-stu-id="917b4-105">Represents how attributes are collected in an identity user flow.</span></span> <span data-ttu-id="917b4-106">Isso permite opções de personalização para coletar atributos dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-106">This allows customization options for collecting attributes within the user flow.</span></span> <span data-ttu-id="917b4-107">Você pode ter várias identidadesUserFlowAttributeAssignments em um único fluxo de usuários que cria a experiência para fornecer as informações necessárias pelo usuário para concluir a assinatura.</span><span class="sxs-lookup"><span data-stu-id="917b4-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience for providing the information required by the user to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="917b4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="917b4-108">Methods</span></span>

|<span data-ttu-id="917b4-109">Método</span><span class="sxs-lookup"><span data-stu-id="917b4-109">Method</span></span>|<span data-ttu-id="917b4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="917b4-110">Return type</span></span>|<span data-ttu-id="917b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="917b4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="917b4-112">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="917b4-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="917b4-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="917b4-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="917b4-114">Leia as propriedades e as relações de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="917b4-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="917b4-115">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="917b4-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="917b4-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="917b4-116">None</span></span>|<span data-ttu-id="917b4-117">Atualize as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="917b4-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="917b4-118">Excluir identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="917b4-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="917b4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="917b4-119">None</span></span>|<span data-ttu-id="917b4-120">Exclua um objeto identityUserFlowAttributeAssignment específico.</span><span class="sxs-lookup"><span data-stu-id="917b4-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="917b4-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="917b4-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="917b4-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="917b4-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="917b4-123">Obtém a ordem da identityUserFlowAttributes sendo coletada dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="917b4-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="917b4-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="917b4-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="917b4-125">None</span></span>|<span data-ttu-id="917b4-126">Define a ordem da identidadeUserFlowAttributes sendo coletada dentro de um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="917b4-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="917b4-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="917b4-127">Properties</span></span>

|<span data-ttu-id="917b4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="917b4-128">Property</span></span>|<span data-ttu-id="917b4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="917b4-129">Type</span></span>|<span data-ttu-id="917b4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="917b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="917b4-131">id</span><span class="sxs-lookup"><span data-stu-id="917b4-131">id</span></span>|<span data-ttu-id="917b4-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="917b4-132">String</span></span>|<span data-ttu-id="917b4-133">O identificador da identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="917b4-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="917b4-134">Esse identificador é imutável depois de criado.</span><span class="sxs-lookup"><span data-stu-id="917b4-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="917b4-135">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="917b4-135">This is a read-only property.</span></span>|
|<span data-ttu-id="917b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="917b4-136">displayName</span></span>|<span data-ttu-id="917b4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="917b4-137">String</span></span>|<span data-ttu-id="917b4-138">O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="917b4-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="917b4-139">isOptional</span></span>|<span data-ttu-id="917b4-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="917b4-140">Boolean</span></span>|<span data-ttu-id="917b4-141">Determina se identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="917b4-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="917b4-142">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="917b4-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="917b4-143">`false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="917b4-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="917b4-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="917b4-144">requiresVerification</span></span>|<span data-ttu-id="917b4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="917b4-145">Boolean</span></span>|<span data-ttu-id="917b4-146">Determina se identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="917b4-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="917b4-147">Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="917b4-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="917b4-148">userAttributeValues</span></span>|<span data-ttu-id="917b4-149">[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="917b4-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="917b4-150">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="917b4-151">Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="917b4-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="917b4-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="917b4-152">userInputType</span></span>|<span data-ttu-id="917b4-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="917b4-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="917b4-154">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="917b4-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="917b4-155">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="917b4-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="917b4-156">Relações</span><span class="sxs-lookup"><span data-stu-id="917b4-156">Relationships</span></span>

|<span data-ttu-id="917b4-157">Relação</span><span class="sxs-lookup"><span data-stu-id="917b4-157">Relationship</span></span>|<span data-ttu-id="917b4-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="917b4-158">Type</span></span>|<span data-ttu-id="917b4-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="917b4-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="917b4-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="917b4-160">userAttribute</span></span>|[<span data-ttu-id="917b4-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="917b4-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="917b4-162">O atributo do usuário que você deseja adicionar ao seu fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="917b4-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="917b4-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="917b4-163">JSON representation</span></span>

<span data-ttu-id="917b4-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="917b4-164">The following is a JSON representation of the resource.</span></span>
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
