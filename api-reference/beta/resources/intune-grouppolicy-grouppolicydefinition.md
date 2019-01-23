---
title: tipo de recurso de groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma diretiva de grupo único.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429195"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="66d3f-103">tipo de recurso de groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="66d3f-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="66d3f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="66d3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66d3f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66d3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66d3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="66d3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d3f-107">A entidade descreve todas as informações sobre uma diretiva de grupo único.</span><span class="sxs-lookup"><span data-stu-id="66d3f-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="66d3f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="66d3f-108">Methods</span></span>
|<span data-ttu-id="66d3f-109">Método</span><span class="sxs-lookup"><span data-stu-id="66d3f-109">Method</span></span>|<span data-ttu-id="66d3f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66d3f-110">Return Type</span></span>|<span data-ttu-id="66d3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d3f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66d3f-112">Obter groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="66d3f-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="66d3f-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="66d3f-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="66d3f-114">Leia as propriedades e os relacionamentos do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="66d3f-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="66d3f-115">Atualizar groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="66d3f-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="66d3f-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="66d3f-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="66d3f-117">Atualize as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="66d3f-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66d3f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66d3f-118">Properties</span></span>
|<span data-ttu-id="66d3f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66d3f-119">Property</span></span>|<span data-ttu-id="66d3f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d3f-120">Type</span></span>|<span data-ttu-id="66d3f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d3f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d3f-122">classType</span><span class="sxs-lookup"><span data-stu-id="66d3f-122">classType</span></span>|[<span data-ttu-id="66d3f-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="66d3f-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="66d3f-124">Identifica o tipo dos grupos a que a diretiva pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="66d3f-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="66d3f-125">Os valores possíveis são: `user`, `machine`, `both`.</span><span class="sxs-lookup"><span data-stu-id="66d3f-125">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="66d3f-126">displayName</span><span class="sxs-lookup"><span data-stu-id="66d3f-126">displayName</span></span>|<span data-ttu-id="66d3f-127">String</span><span class="sxs-lookup"><span data-stu-id="66d3f-127">String</span></span>|<span data-ttu-id="66d3f-128">O nome da política localizado.</span><span class="sxs-lookup"><span data-stu-id="66d3f-128">The localized policy name.</span></span>|
|<span data-ttu-id="66d3f-129">explainText</span><span class="sxs-lookup"><span data-stu-id="66d3f-129">explainText</span></span>|<span data-ttu-id="66d3f-130">String</span><span class="sxs-lookup"><span data-stu-id="66d3f-130">String</span></span>|<span data-ttu-id="66d3f-131">A explicação ou ajuda texto localizado associado à política.</span><span class="sxs-lookup"><span data-stu-id="66d3f-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="66d3f-132">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="66d3f-132">The default value is empty.</span></span>|
|<span data-ttu-id="66d3f-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="66d3f-133">categoryPath</span></span>|<span data-ttu-id="66d3f-134">String</span><span class="sxs-lookup"><span data-stu-id="66d3f-134">String</span></span>|<span data-ttu-id="66d3f-135">O caminho de categoria completo localizado para a política.</span><span class="sxs-lookup"><span data-stu-id="66d3f-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="66d3f-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="66d3f-136">supportedOn</span></span>|<span data-ttu-id="66d3f-137">String</span><span class="sxs-lookup"><span data-stu-id="66d3f-137">String</span></span>|<span data-ttu-id="66d3f-138">A cadeia de caracteres localizada é usada para especificar qual sistema operacional ou a versão do aplicativo é afetada pela diretiva.</span><span class="sxs-lookup"><span data-stu-id="66d3f-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="66d3f-139">policyType</span><span class="sxs-lookup"><span data-stu-id="66d3f-139">policyType</span></span>|[<span data-ttu-id="66d3f-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="66d3f-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="66d3f-141">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="66d3f-141">Specifies the type of group policy.</span></span> <span data-ttu-id="66d3f-142">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="66d3f-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="66d3f-143">id</span><span class="sxs-lookup"><span data-stu-id="66d3f-143">id</span></span>|<span data-ttu-id="66d3f-144">String</span><span class="sxs-lookup"><span data-stu-id="66d3f-144">String</span></span>|<span data-ttu-id="66d3f-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="66d3f-145">Key of the entity.</span></span>|
|<span data-ttu-id="66d3f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66d3f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="66d3f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d3f-147">DateTimeOffset</span></span>|<span data-ttu-id="66d3f-148">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="66d3f-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d3f-149">Relações</span><span class="sxs-lookup"><span data-stu-id="66d3f-149">Relationships</span></span>
|<span data-ttu-id="66d3f-150">Relação</span><span class="sxs-lookup"><span data-stu-id="66d3f-150">Relationship</span></span>|<span data-ttu-id="66d3f-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d3f-151">Type</span></span>|<span data-ttu-id="66d3f-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d3f-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d3f-153">definitionFile</span><span class="sxs-lookup"><span data-stu-id="66d3f-153">definitionFile</span></span>|[<span data-ttu-id="66d3f-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="66d3f-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="66d3f-155">O arquivo de diretiva de grupo associado à definição.</span><span class="sxs-lookup"><span data-stu-id="66d3f-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="66d3f-156">apresentações</span><span class="sxs-lookup"><span data-stu-id="66d3f-156">presentations</span></span>|<span data-ttu-id="66d3f-157">coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="66d3f-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="66d3f-158">As apresentações de diretiva de grupo associadas à definição.</span><span class="sxs-lookup"><span data-stu-id="66d3f-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66d3f-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66d3f-159">JSON Representation</span></span>
<span data-ttu-id="66d3f-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66d3f-160">Here is a JSON representation of the resource.</span></span>
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




