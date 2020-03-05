---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 038647f4e40036db89ecf61cdece531662658c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528090"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="69cc1-103">tipo de recurso groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="69cc1-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="69cc1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69cc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69cc1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69cc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69cc1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69cc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69cc1-107">A entidade descreve todas as informações sobre uma única diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="69cc1-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="69cc1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="69cc1-108">Methods</span></span>
|<span data-ttu-id="69cc1-109">Método</span><span class="sxs-lookup"><span data-stu-id="69cc1-109">Method</span></span>|<span data-ttu-id="69cc1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69cc1-110">Return Type</span></span>|<span data-ttu-id="69cc1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69cc1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69cc1-112">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="69cc1-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="69cc1-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="69cc1-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="69cc1-114">Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="69cc1-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="69cc1-115">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="69cc1-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="69cc1-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="69cc1-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="69cc1-117">Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="69cc1-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69cc1-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69cc1-118">Properties</span></span>
|<span data-ttu-id="69cc1-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69cc1-119">Property</span></span>|<span data-ttu-id="69cc1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="69cc1-120">Type</span></span>|<span data-ttu-id="69cc1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="69cc1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cc1-122">classType</span><span class="sxs-lookup"><span data-stu-id="69cc1-122">classType</span></span>|[<span data-ttu-id="69cc1-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="69cc1-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="69cc1-124">Identifica o tipo de grupo ao qual a política pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="69cc1-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="69cc1-125">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="69cc1-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="69cc1-126">displayName</span><span class="sxs-lookup"><span data-stu-id="69cc1-126">displayName</span></span>|<span data-ttu-id="69cc1-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69cc1-127">String</span></span>|<span data-ttu-id="69cc1-128">O nome da política localizada.</span><span class="sxs-lookup"><span data-stu-id="69cc1-128">The localized policy name.</span></span>|
|<span data-ttu-id="69cc1-129">Texto não criptografado</span><span class="sxs-lookup"><span data-stu-id="69cc1-129">explainText</span></span>|<span data-ttu-id="69cc1-130">String</span><span class="sxs-lookup"><span data-stu-id="69cc1-130">String</span></span>|<span data-ttu-id="69cc1-131">A explicação localizada ou o texto de ajuda associado à política.</span><span class="sxs-lookup"><span data-stu-id="69cc1-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="69cc1-132">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="69cc1-132">The default value is empty.</span></span>|
|<span data-ttu-id="69cc1-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="69cc1-133">categoryPath</span></span>|<span data-ttu-id="69cc1-134">String</span><span class="sxs-lookup"><span data-stu-id="69cc1-134">String</span></span>|<span data-ttu-id="69cc1-135">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="69cc1-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="69cc1-136">com suporte</span><span class="sxs-lookup"><span data-stu-id="69cc1-136">supportedOn</span></span>|<span data-ttu-id="69cc1-137">String</span><span class="sxs-lookup"><span data-stu-id="69cc1-137">String</span></span>|<span data-ttu-id="69cc1-138">Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.</span><span class="sxs-lookup"><span data-stu-id="69cc1-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="69cc1-139">PolicyType</span><span class="sxs-lookup"><span data-stu-id="69cc1-139">policyType</span></span>|[<span data-ttu-id="69cc1-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="69cc1-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="69cc1-141">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="69cc1-141">Specifies the type of group policy.</span></span> <span data-ttu-id="69cc1-142">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="69cc1-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="69cc1-143">id</span><span class="sxs-lookup"><span data-stu-id="69cc1-143">id</span></span>|<span data-ttu-id="69cc1-144">String</span><span class="sxs-lookup"><span data-stu-id="69cc1-144">String</span></span>|<span data-ttu-id="69cc1-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69cc1-145">Key of the entity.</span></span>|
|<span data-ttu-id="69cc1-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69cc1-146">lastModifiedDateTime</span></span>|<span data-ttu-id="69cc1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69cc1-147">DateTimeOffset</span></span>|<span data-ttu-id="69cc1-148">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="69cc1-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69cc1-149">Relações</span><span class="sxs-lookup"><span data-stu-id="69cc1-149">Relationships</span></span>
|<span data-ttu-id="69cc1-150">Relação</span><span class="sxs-lookup"><span data-stu-id="69cc1-150">Relationship</span></span>|<span data-ttu-id="69cc1-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="69cc1-151">Type</span></span>|<span data-ttu-id="69cc1-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="69cc1-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cc1-153">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="69cc1-153">definitionFile</span></span>|[<span data-ttu-id="69cc1-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="69cc1-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="69cc1-155">O arquivo de política de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="69cc1-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="69cc1-156">apresentações</span><span class="sxs-lookup"><span data-stu-id="69cc1-156">presentations</span></span>|<span data-ttu-id="69cc1-157">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="69cc1-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="69cc1-158">As apresentações de política de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="69cc1-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69cc1-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69cc1-159">JSON Representation</span></span>
<span data-ttu-id="69cc1-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69cc1-160">Here is a JSON representation of the resource.</span></span>
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



