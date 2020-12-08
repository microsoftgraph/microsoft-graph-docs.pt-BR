---
title: tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usados para coletar identityUserFlowAttributes específicos dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581277"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="325e8-103">tipo de recurso identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="325e8-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="325e8-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="325e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="325e8-105">identityUserFlowAttributeAssignments são usados para coletar identityUserFlowAttributes específicos dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="325e8-106">Isso permite o controle sobre os atributos coletados em um fluxo de usuário e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="325e8-107">Você pode ter vários identityUserFlowAttributeAssignments em um único fluxo de usuário que cria a experiência que o usuário final vê durante a inscrição quando solicitado a fornecer as informações exigidas pelo fluxo de usuário para concluir a inscrição.</span><span class="sxs-lookup"><span data-stu-id="325e8-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="325e8-108">Methods</span><span class="sxs-lookup"><span data-stu-id="325e8-108">Methods</span></span>

|<span data-ttu-id="325e8-109">Método</span><span class="sxs-lookup"><span data-stu-id="325e8-109">Method</span></span>|<span data-ttu-id="325e8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="325e8-110">Return type</span></span>|<span data-ttu-id="325e8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="325e8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="325e8-112">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="325e8-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="325e8-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="325e8-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="325e8-114">Leia as propriedades e os relacionamentos de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="325e8-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="325e8-115">Atualizar identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="325e8-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="325e8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="325e8-116">None</span></span>|<span data-ttu-id="325e8-117">Atualiza as propriedades de um objeto identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="325e8-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="325e8-118">Excluir identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="325e8-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="325e8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="325e8-119">None</span></span>|<span data-ttu-id="325e8-120">Excluir um objeto identityUserFlowAttributeAssignment específico.</span><span class="sxs-lookup"><span data-stu-id="325e8-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="325e8-121">GetOrder</span><span class="sxs-lookup"><span data-stu-id="325e8-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="325e8-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="325e8-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="325e8-123">Obtém a ordem do identityUserFlowAttributes que está sendo coletado dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="325e8-124">SetOrder</span><span class="sxs-lookup"><span data-stu-id="325e8-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="325e8-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="325e8-125">None</span></span>|<span data-ttu-id="325e8-126">Define a ordem de coleta de identityUserFlowAttributes em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="325e8-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="325e8-127">Properties</span></span>

|<span data-ttu-id="325e8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="325e8-128">Property</span></span>|<span data-ttu-id="325e8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="325e8-129">Type</span></span>|<span data-ttu-id="325e8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="325e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="325e8-131">id</span><span class="sxs-lookup"><span data-stu-id="325e8-131">id</span></span>|<span data-ttu-id="325e8-132">String</span><span class="sxs-lookup"><span data-stu-id="325e8-132">String</span></span>|<span data-ttu-id="325e8-133">O identificador do identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="325e8-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="325e8-134">Esse identificador é imutável após sua criação.</span><span class="sxs-lookup"><span data-stu-id="325e8-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="325e8-135">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="325e8-135">This is a read-only property.</span></span>|
|<span data-ttu-id="325e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="325e8-136">displayName</span></span>|<span data-ttu-id="325e8-137">String</span><span class="sxs-lookup"><span data-stu-id="325e8-137">String</span></span>|<span data-ttu-id="325e8-138">O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="325e8-139">IsOptional</span><span class="sxs-lookup"><span data-stu-id="325e8-139">isOptional</span></span>|<span data-ttu-id="325e8-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="325e8-140">Boolean</span></span>|<span data-ttu-id="325e8-141">Determina se o identityUserFlowAttribute é opcional.</span><span class="sxs-lookup"><span data-stu-id="325e8-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="325e8-142">`true` significa que o usuário não precisa fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="325e8-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="325e8-143">`false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.</span><span class="sxs-lookup"><span data-stu-id="325e8-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="325e8-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="325e8-144">requiresVerification</span></span>|<span data-ttu-id="325e8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="325e8-145">Boolean</span></span>|<span data-ttu-id="325e8-146">Determina se o identityUserFlowAttribute requer verificação.</span><span class="sxs-lookup"><span data-stu-id="325e8-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="325e8-147">Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="325e8-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="325e8-148">userAttributeValues</span></span>|<span data-ttu-id="325e8-149">coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="325e8-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="325e8-150">As opções de entrada para o atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="325e8-151">Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="325e8-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="325e8-152">userinputtype</span><span class="sxs-lookup"><span data-stu-id="325e8-152">userInputType</span></span>|<span data-ttu-id="325e8-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="325e8-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="325e8-154">O tipo de entrada do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="325e8-155">Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="325e8-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="325e8-156">Relações</span><span class="sxs-lookup"><span data-stu-id="325e8-156">Relationships</span></span>

|<span data-ttu-id="325e8-157">Relação</span><span class="sxs-lookup"><span data-stu-id="325e8-157">Relationship</span></span>|<span data-ttu-id="325e8-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="325e8-158">Type</span></span>|<span data-ttu-id="325e8-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="325e8-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="325e8-160">userattribute</span><span class="sxs-lookup"><span data-stu-id="325e8-160">userAttribute</span></span>|[<span data-ttu-id="325e8-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="325e8-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="325e8-162">O atributo de usuário que você deseja adicionar ao seu fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="325e8-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="325e8-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="325e8-163">JSON representation</span></span>

<span data-ttu-id="325e8-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="325e8-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
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
