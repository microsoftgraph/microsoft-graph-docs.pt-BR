---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa766eace326dd05470b753f8daf6acfa8362e6f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941132"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="a8a98-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="a8a98-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="a8a98-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8a98-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8a98-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8a98-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8a98-108">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="a8a98-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="a8a98-109">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="a8a98-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="a8a98-110">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="a8a98-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="a8a98-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="a8a98-111">Methods</span></span>
|<span data-ttu-id="a8a98-112">Método</span><span class="sxs-lookup"><span data-stu-id="a8a98-112">Method</span></span>|<span data-ttu-id="a8a98-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a8a98-113">Return Type</span></span>|<span data-ttu-id="a8a98-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a98-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8a98-115">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="a8a98-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="a8a98-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="a8a98-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="a8a98-117">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="a8a98-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="a8a98-118">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="a8a98-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="a8a98-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="a8a98-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="a8a98-120">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="a8a98-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8a98-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8a98-121">Properties</span></span>
|<span data-ttu-id="a8a98-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8a98-122">Property</span></span>|<span data-ttu-id="a8a98-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a98-123">Type</span></span>|<span data-ttu-id="a8a98-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a98-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a98-125">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a98-125">displayName</span></span>|<span data-ttu-id="a8a98-126">String</span><span class="sxs-lookup"><span data-stu-id="a8a98-126">String</span></span>|<span data-ttu-id="a8a98-127">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="a8a98-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="a8a98-128">description</span><span class="sxs-lookup"><span data-stu-id="a8a98-128">description</span></span>|<span data-ttu-id="a8a98-129">String</span><span class="sxs-lookup"><span data-stu-id="a8a98-129">String</span></span>|<span data-ttu-id="a8a98-130">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="a8a98-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="a8a98-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="a8a98-131">The default value is empty.</span></span>|
|<span data-ttu-id="a8a98-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="a8a98-132">languageCodes</span></span>|<span data-ttu-id="a8a98-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a98-133">String collection</span></span>|<span data-ttu-id="a8a98-134">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="a8a98-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="a8a98-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="a8a98-135">targetPrefix</span></span>|<span data-ttu-id="a8a98-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a98-136">String</span></span>|<span data-ttu-id="a8a98-137">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="a8a98-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="a8a98-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="a8a98-138">targetNamespace</span></span>|<span data-ttu-id="a8a98-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a98-139">String</span></span>|<span data-ttu-id="a8a98-140">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="a8a98-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="a8a98-141">PolicyType</span><span class="sxs-lookup"><span data-stu-id="a8a98-141">policyType</span></span>|[<span data-ttu-id="a8a98-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="a8a98-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="a8a98-143">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a8a98-143">Specifies the type of group policy.</span></span> <span data-ttu-id="a8a98-144">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="a8a98-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="a8a98-145">id</span><span class="sxs-lookup"><span data-stu-id="a8a98-145">id</span></span>|<span data-ttu-id="a8a98-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a98-146">String</span></span>|<span data-ttu-id="a8a98-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8a98-147">Key of the entity.</span></span>|
|<span data-ttu-id="a8a98-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a98-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a8a98-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a98-149">DateTimeOffset</span></span>|<span data-ttu-id="a8a98-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a8a98-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8a98-151">Relações</span><span class="sxs-lookup"><span data-stu-id="a8a98-151">Relationships</span></span>
|<span data-ttu-id="a8a98-152">Relação</span><span class="sxs-lookup"><span data-stu-id="a8a98-152">Relationship</span></span>|<span data-ttu-id="a8a98-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a98-153">Type</span></span>|<span data-ttu-id="a8a98-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a98-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a98-155">Definição</span><span class="sxs-lookup"><span data-stu-id="a8a98-155">definitions</span></span>|<span data-ttu-id="a8a98-156">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a8a98-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="a8a98-157">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="a8a98-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8a98-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8a98-158">JSON Representation</span></span>
<span data-ttu-id="a8a98-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8a98-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




