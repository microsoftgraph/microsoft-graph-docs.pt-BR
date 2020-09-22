---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef94f2d5163fad7151b7b39d278438231e62923
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031022"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="09271-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="09271-105">groupPolicyDefinitionFile resource type</span></span>

<span data-ttu-id="09271-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09271-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09271-107">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09271-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09271-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09271-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09271-109">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="09271-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="09271-110">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="09271-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="09271-111">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="09271-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="09271-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="09271-112">Methods</span></span>
|<span data-ttu-id="09271-113">Método</span><span class="sxs-lookup"><span data-stu-id="09271-113">Method</span></span>|<span data-ttu-id="09271-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09271-114">Return Type</span></span>|<span data-ttu-id="09271-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="09271-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09271-116">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="09271-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="09271-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="09271-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="09271-118">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="09271-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="09271-119">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="09271-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="09271-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="09271-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="09271-121">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="09271-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09271-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09271-122">Properties</span></span>
|<span data-ttu-id="09271-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09271-123">Property</span></span>|<span data-ttu-id="09271-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="09271-124">Type</span></span>|<span data-ttu-id="09271-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="09271-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09271-126">displayName</span><span class="sxs-lookup"><span data-stu-id="09271-126">displayName</span></span>|<span data-ttu-id="09271-127">String</span><span class="sxs-lookup"><span data-stu-id="09271-127">String</span></span>|<span data-ttu-id="09271-128">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="09271-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="09271-129">description</span><span class="sxs-lookup"><span data-stu-id="09271-129">description</span></span>|<span data-ttu-id="09271-130">String</span><span class="sxs-lookup"><span data-stu-id="09271-130">String</span></span>|<span data-ttu-id="09271-131">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="09271-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="09271-132">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="09271-132">The default value is empty.</span></span>|
|<span data-ttu-id="09271-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="09271-133">languageCodes</span></span>|<span data-ttu-id="09271-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="09271-134">String collection</span></span>|<span data-ttu-id="09271-135">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="09271-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="09271-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="09271-136">targetPrefix</span></span>|<span data-ttu-id="09271-137">String</span><span class="sxs-lookup"><span data-stu-id="09271-137">String</span></span>|<span data-ttu-id="09271-138">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="09271-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="09271-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="09271-139">targetNamespace</span></span>|<span data-ttu-id="09271-140">String</span><span class="sxs-lookup"><span data-stu-id="09271-140">String</span></span>|<span data-ttu-id="09271-141">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="09271-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="09271-142">PolicyType</span><span class="sxs-lookup"><span data-stu-id="09271-142">policyType</span></span>|[<span data-ttu-id="09271-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="09271-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="09271-144">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="09271-144">Specifies the type of group policy.</span></span> <span data-ttu-id="09271-145">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="09271-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="09271-146">firmware</span><span class="sxs-lookup"><span data-stu-id="09271-146">revision</span></span>|<span data-ttu-id="09271-147">String</span><span class="sxs-lookup"><span data-stu-id="09271-147">String</span></span>|<span data-ttu-id="09271-148">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="09271-148">The revision version associated with the file.</span></span>|
|<span data-ttu-id="09271-149">id</span><span class="sxs-lookup"><span data-stu-id="09271-149">id</span></span>|<span data-ttu-id="09271-150">String</span><span class="sxs-lookup"><span data-stu-id="09271-150">String</span></span>|<span data-ttu-id="09271-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="09271-151">Key of the entity.</span></span>|
|<span data-ttu-id="09271-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09271-152">lastModifiedDateTime</span></span>|<span data-ttu-id="09271-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09271-153">DateTimeOffset</span></span>|<span data-ttu-id="09271-154">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="09271-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09271-155">Relações</span><span class="sxs-lookup"><span data-stu-id="09271-155">Relationships</span></span>
|<span data-ttu-id="09271-156">Relação</span><span class="sxs-lookup"><span data-stu-id="09271-156">Relationship</span></span>|<span data-ttu-id="09271-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="09271-157">Type</span></span>|<span data-ttu-id="09271-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="09271-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09271-159">Definição</span><span class="sxs-lookup"><span data-stu-id="09271-159">definitions</span></span>|<span data-ttu-id="09271-160">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="09271-160">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="09271-161">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="09271-161">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09271-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09271-162">JSON Representation</span></span>
<span data-ttu-id="09271-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09271-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






