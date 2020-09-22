---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9ba5a4c415b0bc94b60479530ac6a7ca35f3c75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031008"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="02fc0-103">tipo de recurso groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="02fc0-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="02fc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02fc0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02fc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02fc0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02fc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02fc0-107">A entidade descreve todas as informações sobre uma única diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="02fc0-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="02fc0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="02fc0-108">Methods</span></span>
|<span data-ttu-id="02fc0-109">Método</span><span class="sxs-lookup"><span data-stu-id="02fc0-109">Method</span></span>|<span data-ttu-id="02fc0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02fc0-110">Return Type</span></span>|<span data-ttu-id="02fc0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fc0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02fc0-112">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="02fc0-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="02fc0-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="02fc0-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="02fc0-114">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="02fc0-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="02fc0-115">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="02fc0-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="02fc0-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="02fc0-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="02fc0-117">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="02fc0-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02fc0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02fc0-118">Properties</span></span>
|<span data-ttu-id="02fc0-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02fc0-119">Property</span></span>|<span data-ttu-id="02fc0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fc0-120">Type</span></span>|<span data-ttu-id="02fc0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fc0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02fc0-122">classType</span><span class="sxs-lookup"><span data-stu-id="02fc0-122">classType</span></span>|[<span data-ttu-id="02fc0-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="02fc0-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="02fc0-124">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="02fc0-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="02fc0-125">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="02fc0-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="02fc0-126">displayName</span><span class="sxs-lookup"><span data-stu-id="02fc0-126">displayName</span></span>|<span data-ttu-id="02fc0-127">String</span><span class="sxs-lookup"><span data-stu-id="02fc0-127">String</span></span>|<span data-ttu-id="02fc0-128">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="02fc0-128">The localized policy name.</span></span>|
|<span data-ttu-id="02fc0-129">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="02fc0-129">explainText</span></span>|<span data-ttu-id="02fc0-130">String</span><span class="sxs-lookup"><span data-stu-id="02fc0-130">String</span></span>|<span data-ttu-id="02fc0-131">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="02fc0-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="02fc0-132">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="02fc0-132">The default value is empty.</span></span>|
|<span data-ttu-id="02fc0-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="02fc0-133">categoryPath</span></span>|<span data-ttu-id="02fc0-134">String</span><span class="sxs-lookup"><span data-stu-id="02fc0-134">String</span></span>|<span data-ttu-id="02fc0-135">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="02fc0-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="02fc0-136">com suporte</span><span class="sxs-lookup"><span data-stu-id="02fc0-136">supportedOn</span></span>|<span data-ttu-id="02fc0-137">String</span><span class="sxs-lookup"><span data-stu-id="02fc0-137">String</span></span>|<span data-ttu-id="02fc0-138">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="02fc0-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="02fc0-139">PolicyType</span><span class="sxs-lookup"><span data-stu-id="02fc0-139">policyType</span></span>|[<span data-ttu-id="02fc0-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="02fc0-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="02fc0-141">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="02fc0-141">Specifies the type of group policy.</span></span> <span data-ttu-id="02fc0-142">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="02fc0-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="02fc0-143">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="02fc0-143">groupPolicyCategoryId</span></span>|<span data-ttu-id="02fc0-144">Guid</span><span class="sxs-lookup"><span data-stu-id="02fc0-144">Guid</span></span>|<span data-ttu-id="02fc0-145">A ID de categoria da categoria pai</span><span class="sxs-lookup"><span data-stu-id="02fc0-145">The category id of the parent category</span></span>|
|<span data-ttu-id="02fc0-146">id</span><span class="sxs-lookup"><span data-stu-id="02fc0-146">id</span></span>|<span data-ttu-id="02fc0-147">String</span><span class="sxs-lookup"><span data-stu-id="02fc0-147">String</span></span>|<span data-ttu-id="02fc0-148">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02fc0-148">Key of the entity.</span></span>|
|<span data-ttu-id="02fc0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02fc0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="02fc0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02fc0-150">DateTimeOffset</span></span>|<span data-ttu-id="02fc0-151">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="02fc0-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02fc0-152">Relações</span><span class="sxs-lookup"><span data-stu-id="02fc0-152">Relationships</span></span>
|<span data-ttu-id="02fc0-153">Relação</span><span class="sxs-lookup"><span data-stu-id="02fc0-153">Relationship</span></span>|<span data-ttu-id="02fc0-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fc0-154">Type</span></span>|<span data-ttu-id="02fc0-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fc0-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02fc0-156">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="02fc0-156">definitionFile</span></span>|[<span data-ttu-id="02fc0-157">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="02fc0-157">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="02fc0-158">O arquivo de política de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="02fc0-158">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="02fc0-159">category</span><span class="sxs-lookup"><span data-stu-id="02fc0-159">category</span></span>|[<span data-ttu-id="02fc0-160">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="02fc0-160">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="02fc0-161">A categoria de política de grupo associada à definição.</span><span class="sxs-lookup"><span data-stu-id="02fc0-161">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="02fc0-162">apresentações</span><span class="sxs-lookup"><span data-stu-id="02fc0-162">presentations</span></span>|<span data-ttu-id="02fc0-163">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="02fc0-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="02fc0-164">As apresentações de política de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="02fc0-164">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02fc0-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02fc0-165">JSON Representation</span></span>
<span data-ttu-id="02fc0-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02fc0-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






