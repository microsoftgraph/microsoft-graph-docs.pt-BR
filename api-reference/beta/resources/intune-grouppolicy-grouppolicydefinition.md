---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a68740101c79efda08f010b6e8410428c883bb2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998678"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="71285-103">tipo de recurso groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="71285-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="71285-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71285-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71285-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71285-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71285-106">A entidade descreve todas as informações sobre uma única diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="71285-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="71285-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="71285-107">Methods</span></span>
|<span data-ttu-id="71285-108">Método</span><span class="sxs-lookup"><span data-stu-id="71285-108">Method</span></span>|<span data-ttu-id="71285-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71285-109">Return Type</span></span>|<span data-ttu-id="71285-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71285-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71285-111">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="71285-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="71285-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="71285-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="71285-113">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="71285-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="71285-114">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="71285-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="71285-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="71285-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="71285-116">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="71285-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71285-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71285-117">Properties</span></span>
|<span data-ttu-id="71285-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71285-118">Property</span></span>|<span data-ttu-id="71285-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="71285-119">Type</span></span>|<span data-ttu-id="71285-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71285-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71285-121">classType</span><span class="sxs-lookup"><span data-stu-id="71285-121">classType</span></span>|[<span data-ttu-id="71285-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="71285-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="71285-123">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="71285-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="71285-124">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="71285-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="71285-125">displayName</span><span class="sxs-lookup"><span data-stu-id="71285-125">displayName</span></span>|<span data-ttu-id="71285-126">String</span><span class="sxs-lookup"><span data-stu-id="71285-126">String</span></span>|<span data-ttu-id="71285-127">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="71285-127">The localized policy name.</span></span>|
|<span data-ttu-id="71285-128">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="71285-128">explainText</span></span>|<span data-ttu-id="71285-129">String</span><span class="sxs-lookup"><span data-stu-id="71285-129">String</span></span>|<span data-ttu-id="71285-130">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="71285-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="71285-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="71285-131">The default value is empty.</span></span>|
|<span data-ttu-id="71285-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="71285-132">categoryPath</span></span>|<span data-ttu-id="71285-133">String</span><span class="sxs-lookup"><span data-stu-id="71285-133">String</span></span>|<span data-ttu-id="71285-134">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="71285-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="71285-135">com suporte</span><span class="sxs-lookup"><span data-stu-id="71285-135">supportedOn</span></span>|<span data-ttu-id="71285-136">String</span><span class="sxs-lookup"><span data-stu-id="71285-136">String</span></span>|<span data-ttu-id="71285-137">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="71285-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="71285-138">PolicyType</span><span class="sxs-lookup"><span data-stu-id="71285-138">policyType</span></span>|[<span data-ttu-id="71285-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="71285-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="71285-140">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="71285-140">Specifies the type of group policy.</span></span> <span data-ttu-id="71285-141">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="71285-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="71285-142">id</span><span class="sxs-lookup"><span data-stu-id="71285-142">id</span></span>|<span data-ttu-id="71285-143">String</span><span class="sxs-lookup"><span data-stu-id="71285-143">String</span></span>|<span data-ttu-id="71285-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71285-144">Key of the entity.</span></span>|
|<span data-ttu-id="71285-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71285-145">lastModifiedDateTime</span></span>|<span data-ttu-id="71285-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71285-146">DateTimeOffset</span></span>|<span data-ttu-id="71285-147">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="71285-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71285-148">Relações</span><span class="sxs-lookup"><span data-stu-id="71285-148">Relationships</span></span>
|<span data-ttu-id="71285-149">Relação</span><span class="sxs-lookup"><span data-stu-id="71285-149">Relationship</span></span>|<span data-ttu-id="71285-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="71285-150">Type</span></span>|<span data-ttu-id="71285-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="71285-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71285-152">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="71285-152">definitionFile</span></span>|[<span data-ttu-id="71285-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="71285-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="71285-154">O arquivo de política de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="71285-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="71285-155">apresentações</span><span class="sxs-lookup"><span data-stu-id="71285-155">presentations</span></span>|<span data-ttu-id="71285-156">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="71285-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="71285-157">As apresentações de política de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="71285-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71285-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71285-158">JSON Representation</span></span>
<span data-ttu-id="71285-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71285-159">Here is a JSON representation of the resource.</span></span>
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





