---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e38daccc28f3525b0efc80586b71d7ac62359616
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975879"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="f3775-103">tipo de recurso groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f3775-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="f3775-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3775-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3775-106">A entidade descreve todas as informações sobre uma única diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="f3775-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="f3775-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3775-107">Methods</span></span>
|<span data-ttu-id="f3775-108">Método</span><span class="sxs-lookup"><span data-stu-id="f3775-108">Method</span></span>|<span data-ttu-id="f3775-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3775-109">Return Type</span></span>|<span data-ttu-id="f3775-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3775-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3775-111">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f3775-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="f3775-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f3775-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="f3775-113">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f3775-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="f3775-114">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f3775-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="f3775-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f3775-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="f3775-116">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f3775-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3775-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3775-117">Properties</span></span>
|<span data-ttu-id="f3775-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3775-118">Property</span></span>|<span data-ttu-id="f3775-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3775-119">Type</span></span>|<span data-ttu-id="f3775-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3775-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3775-121">classType</span><span class="sxs-lookup"><span data-stu-id="f3775-121">classType</span></span>|[<span data-ttu-id="f3775-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="f3775-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="f3775-123">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="f3775-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="f3775-124">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f3775-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f3775-125">displayName</span><span class="sxs-lookup"><span data-stu-id="f3775-125">displayName</span></span>|<span data-ttu-id="f3775-126">String</span><span class="sxs-lookup"><span data-stu-id="f3775-126">String</span></span>|<span data-ttu-id="f3775-127">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="f3775-127">The localized policy name.</span></span>|
|<span data-ttu-id="f3775-128">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="f3775-128">explainText</span></span>|<span data-ttu-id="f3775-129">String</span><span class="sxs-lookup"><span data-stu-id="f3775-129">String</span></span>|<span data-ttu-id="f3775-130">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="f3775-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="f3775-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="f3775-131">The default value is empty.</span></span>|
|<span data-ttu-id="f3775-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="f3775-132">categoryPath</span></span>|<span data-ttu-id="f3775-133">String</span><span class="sxs-lookup"><span data-stu-id="f3775-133">String</span></span>|<span data-ttu-id="f3775-134">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="f3775-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="f3775-135">com suporte</span><span class="sxs-lookup"><span data-stu-id="f3775-135">supportedOn</span></span>|<span data-ttu-id="f3775-136">String</span><span class="sxs-lookup"><span data-stu-id="f3775-136">String</span></span>|<span data-ttu-id="f3775-137">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="f3775-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="f3775-138">PolicyType</span><span class="sxs-lookup"><span data-stu-id="f3775-138">policyType</span></span>|[<span data-ttu-id="f3775-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="f3775-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="f3775-140">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f3775-140">Specifies the type of group policy.</span></span> <span data-ttu-id="f3775-141">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="f3775-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="f3775-142">id</span><span class="sxs-lookup"><span data-stu-id="f3775-142">id</span></span>|<span data-ttu-id="f3775-143">String</span><span class="sxs-lookup"><span data-stu-id="f3775-143">String</span></span>|<span data-ttu-id="f3775-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3775-144">Key of the entity.</span></span>|
|<span data-ttu-id="f3775-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3775-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f3775-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3775-146">DateTimeOffset</span></span>|<span data-ttu-id="f3775-147">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f3775-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3775-148">Relações</span><span class="sxs-lookup"><span data-stu-id="f3775-148">Relationships</span></span>
|<span data-ttu-id="f3775-149">Relação</span><span class="sxs-lookup"><span data-stu-id="f3775-149">Relationship</span></span>|<span data-ttu-id="f3775-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3775-150">Type</span></span>|<span data-ttu-id="f3775-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3775-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3775-152">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="f3775-152">definitionFile</span></span>|[<span data-ttu-id="f3775-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="f3775-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="f3775-154">O arquivo de política de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="f3775-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="f3775-155">apresentações</span><span class="sxs-lookup"><span data-stu-id="f3775-155">presentations</span></span>|<span data-ttu-id="f3775-156">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f3775-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="f3775-157">As apresentações de política de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="f3775-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3775-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3775-158">JSON Representation</span></span>
<span data-ttu-id="f3775-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3775-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





