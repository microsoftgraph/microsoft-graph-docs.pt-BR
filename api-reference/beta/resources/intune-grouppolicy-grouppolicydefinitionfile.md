---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 384b59a2c9e1b669cd71b294c6420c13b95d1102
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576484"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="ee84b-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="ee84b-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="ee84b-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee84b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee84b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee84b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee84b-108">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="ee84b-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="ee84b-109">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="ee84b-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="ee84b-110">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="ee84b-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="ee84b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee84b-111">Methods</span></span>
|<span data-ttu-id="ee84b-112">Método</span><span class="sxs-lookup"><span data-stu-id="ee84b-112">Method</span></span>|<span data-ttu-id="ee84b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee84b-113">Return Type</span></span>|<span data-ttu-id="ee84b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee84b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee84b-115">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="ee84b-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="ee84b-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="ee84b-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="ee84b-117">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="ee84b-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="ee84b-118">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="ee84b-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="ee84b-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="ee84b-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="ee84b-120">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="ee84b-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee84b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee84b-121">Properties</span></span>
|<span data-ttu-id="ee84b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee84b-122">Property</span></span>|<span data-ttu-id="ee84b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee84b-123">Type</span></span>|<span data-ttu-id="ee84b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee84b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee84b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="ee84b-125">displayName</span></span>|<span data-ttu-id="ee84b-126">String</span><span class="sxs-lookup"><span data-stu-id="ee84b-126">String</span></span>|<span data-ttu-id="ee84b-127">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ee84b-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="ee84b-128">descrição</span><span class="sxs-lookup"><span data-stu-id="ee84b-128">description</span></span>|<span data-ttu-id="ee84b-129">String</span><span class="sxs-lookup"><span data-stu-id="ee84b-129">String</span></span>|<span data-ttu-id="ee84b-130">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ee84b-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="ee84b-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="ee84b-131">The default value is empty.</span></span>|
|<span data-ttu-id="ee84b-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="ee84b-132">languageCodes</span></span>|<span data-ttu-id="ee84b-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee84b-133">String collection</span></span>|<span data-ttu-id="ee84b-134">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ee84b-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="ee84b-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="ee84b-135">targetPrefix</span></span>|<span data-ttu-id="ee84b-136">String</span><span class="sxs-lookup"><span data-stu-id="ee84b-136">String</span></span>|<span data-ttu-id="ee84b-137">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ee84b-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="ee84b-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="ee84b-138">targetNamespace</span></span>|<span data-ttu-id="ee84b-139">String</span><span class="sxs-lookup"><span data-stu-id="ee84b-139">String</span></span>|<span data-ttu-id="ee84b-140">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="ee84b-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="ee84b-141">PolicyType</span><span class="sxs-lookup"><span data-stu-id="ee84b-141">policyType</span></span>|[<span data-ttu-id="ee84b-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="ee84b-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="ee84b-143">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="ee84b-143">Specifies the type of group policy.</span></span> <span data-ttu-id="ee84b-144">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="ee84b-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="ee84b-145">firmware</span><span class="sxs-lookup"><span data-stu-id="ee84b-145">revision</span></span>|<span data-ttu-id="ee84b-146">String</span><span class="sxs-lookup"><span data-stu-id="ee84b-146">String</span></span>|<span data-ttu-id="ee84b-147">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee84b-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="ee84b-148">id</span><span class="sxs-lookup"><span data-stu-id="ee84b-148">id</span></span>|<span data-ttu-id="ee84b-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee84b-149">String</span></span>|<span data-ttu-id="ee84b-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee84b-150">Key of the entity.</span></span>|
|<span data-ttu-id="ee84b-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee84b-151">lastModifiedDateTime</span></span>|<span data-ttu-id="ee84b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee84b-152">DateTimeOffset</span></span>|<span data-ttu-id="ee84b-153">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ee84b-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee84b-154">Relações</span><span class="sxs-lookup"><span data-stu-id="ee84b-154">Relationships</span></span>
|<span data-ttu-id="ee84b-155">Relação</span><span class="sxs-lookup"><span data-stu-id="ee84b-155">Relationship</span></span>|<span data-ttu-id="ee84b-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee84b-156">Type</span></span>|<span data-ttu-id="ee84b-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee84b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee84b-158">Definição</span><span class="sxs-lookup"><span data-stu-id="ee84b-158">definitions</span></span>|<span data-ttu-id="ee84b-159">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ee84b-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="ee84b-160">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee84b-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee84b-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee84b-161">JSON Representation</span></span>
<span data-ttu-id="ee84b-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee84b-162">Here is a JSON representation of the resource.</span></span>
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



