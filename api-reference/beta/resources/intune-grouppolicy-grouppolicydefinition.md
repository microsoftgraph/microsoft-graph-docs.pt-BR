---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e99b32687c0a93673cdbf8889b05e6423cc73c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783020"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="fc2cb-103">tipo de recurso groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="fc2cb-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="fc2cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc2cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2cb-106">A entidade descreve todas as informações sobre uma única diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="fc2cb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc2cb-107">Methods</span></span>
|<span data-ttu-id="fc2cb-108">Método</span><span class="sxs-lookup"><span data-stu-id="fc2cb-108">Method</span></span>|<span data-ttu-id="fc2cb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc2cb-109">Return Type</span></span>|<span data-ttu-id="fc2cb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2cb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc2cb-111">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="fc2cb-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="fc2cb-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="fc2cb-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="fc2cb-113">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="fc2cb-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="fc2cb-114">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="fc2cb-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="fc2cb-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="fc2cb-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="fc2cb-116">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="fc2cb-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc2cb-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc2cb-117">Properties</span></span>
|<span data-ttu-id="fc2cb-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc2cb-118">Property</span></span>|<span data-ttu-id="fc2cb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc2cb-119">Type</span></span>|<span data-ttu-id="fc2cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2cb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2cb-121">classType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-121">classType</span></span>|[<span data-ttu-id="fc2cb-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="fc2cb-123">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="fc2cb-124">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="fc2cb-125">displayName</span><span class="sxs-lookup"><span data-stu-id="fc2cb-125">displayName</span></span>|<span data-ttu-id="fc2cb-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc2cb-126">String</span></span>|<span data-ttu-id="fc2cb-127">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-127">The localized policy name.</span></span>|
|<span data-ttu-id="fc2cb-128">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="fc2cb-128">explainText</span></span>|<span data-ttu-id="fc2cb-129">String</span><span class="sxs-lookup"><span data-stu-id="fc2cb-129">String</span></span>|<span data-ttu-id="fc2cb-130">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="fc2cb-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-131">The default value is empty.</span></span>|
|<span data-ttu-id="fc2cb-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="fc2cb-132">categoryPath</span></span>|<span data-ttu-id="fc2cb-133">String</span><span class="sxs-lookup"><span data-stu-id="fc2cb-133">String</span></span>|<span data-ttu-id="fc2cb-134">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="fc2cb-135">com suporte</span><span class="sxs-lookup"><span data-stu-id="fc2cb-135">supportedOn</span></span>|<span data-ttu-id="fc2cb-136">String</span><span class="sxs-lookup"><span data-stu-id="fc2cb-136">String</span></span>|<span data-ttu-id="fc2cb-137">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="fc2cb-138">PolicyType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-138">policyType</span></span>|[<span data-ttu-id="fc2cb-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="fc2cb-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="fc2cb-140">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-140">Specifies the type of group policy.</span></span> <span data-ttu-id="fc2cb-141">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="fc2cb-142">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="fc2cb-142">groupPolicyCategoryId</span></span>|<span data-ttu-id="fc2cb-143">Guid</span><span class="sxs-lookup"><span data-stu-id="fc2cb-143">Guid</span></span>|<span data-ttu-id="fc2cb-144">A ID de categoria da categoria pai</span><span class="sxs-lookup"><span data-stu-id="fc2cb-144">The category id of the parent category</span></span>|
|<span data-ttu-id="fc2cb-145">id</span><span class="sxs-lookup"><span data-stu-id="fc2cb-145">id</span></span>|<span data-ttu-id="fc2cb-146">String</span><span class="sxs-lookup"><span data-stu-id="fc2cb-146">String</span></span>|<span data-ttu-id="fc2cb-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-147">Key of the entity.</span></span>|
|<span data-ttu-id="fc2cb-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc2cb-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fc2cb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc2cb-149">DateTimeOffset</span></span>|<span data-ttu-id="fc2cb-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc2cb-151">Relações</span><span class="sxs-lookup"><span data-stu-id="fc2cb-151">Relationships</span></span>
|<span data-ttu-id="fc2cb-152">Relação</span><span class="sxs-lookup"><span data-stu-id="fc2cb-152">Relationship</span></span>|<span data-ttu-id="fc2cb-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc2cb-153">Type</span></span>|<span data-ttu-id="fc2cb-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2cb-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2cb-155">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fc2cb-155">definitionFile</span></span>|[<span data-ttu-id="fc2cb-156">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fc2cb-156">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="fc2cb-157">O arquivo de política de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-157">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="fc2cb-158">category</span><span class="sxs-lookup"><span data-stu-id="fc2cb-158">category</span></span>|[<span data-ttu-id="fc2cb-159">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="fc2cb-159">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="fc2cb-160">A categoria de política de grupo associada à definição.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-160">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="fc2cb-161">apresentações</span><span class="sxs-lookup"><span data-stu-id="fc2cb-161">presentations</span></span>|<span data-ttu-id="fc2cb-162">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fc2cb-162">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="fc2cb-163">As apresentações de política de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-163">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc2cb-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc2cb-164">JSON Representation</span></span>
<span data-ttu-id="fc2cb-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc2cb-165">Here is a JSON representation of the resource.</span></span>
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



