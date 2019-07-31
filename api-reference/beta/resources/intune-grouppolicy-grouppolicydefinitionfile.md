---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60001517f635352ea2717033279ebebc8df7895b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998622"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="623ae-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="623ae-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="623ae-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="623ae-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="623ae-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="623ae-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623ae-108">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="623ae-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="623ae-109">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="623ae-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="623ae-110">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="623ae-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="623ae-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="623ae-111">Methods</span></span>
|<span data-ttu-id="623ae-112">Método</span><span class="sxs-lookup"><span data-stu-id="623ae-112">Method</span></span>|<span data-ttu-id="623ae-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="623ae-113">Return Type</span></span>|<span data-ttu-id="623ae-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="623ae-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="623ae-115">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="623ae-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="623ae-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="623ae-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="623ae-117">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="623ae-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="623ae-118">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="623ae-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="623ae-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="623ae-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="623ae-120">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="623ae-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="623ae-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="623ae-121">Properties</span></span>
|<span data-ttu-id="623ae-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="623ae-122">Property</span></span>|<span data-ttu-id="623ae-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="623ae-123">Type</span></span>|<span data-ttu-id="623ae-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="623ae-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623ae-125">displayName</span><span class="sxs-lookup"><span data-stu-id="623ae-125">displayName</span></span>|<span data-ttu-id="623ae-126">String</span><span class="sxs-lookup"><span data-stu-id="623ae-126">String</span></span>|<span data-ttu-id="623ae-127">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="623ae-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="623ae-128">descrição</span><span class="sxs-lookup"><span data-stu-id="623ae-128">description</span></span>|<span data-ttu-id="623ae-129">String</span><span class="sxs-lookup"><span data-stu-id="623ae-129">String</span></span>|<span data-ttu-id="623ae-130">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="623ae-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="623ae-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="623ae-131">The default value is empty.</span></span>|
|<span data-ttu-id="623ae-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="623ae-132">languageCodes</span></span>|<span data-ttu-id="623ae-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="623ae-133">String collection</span></span>|<span data-ttu-id="623ae-134">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="623ae-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="623ae-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="623ae-135">targetPrefix</span></span>|<span data-ttu-id="623ae-136">String</span><span class="sxs-lookup"><span data-stu-id="623ae-136">String</span></span>|<span data-ttu-id="623ae-137">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="623ae-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="623ae-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="623ae-138">targetNamespace</span></span>|<span data-ttu-id="623ae-139">String</span><span class="sxs-lookup"><span data-stu-id="623ae-139">String</span></span>|<span data-ttu-id="623ae-140">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="623ae-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="623ae-141">PolicyType</span><span class="sxs-lookup"><span data-stu-id="623ae-141">policyType</span></span>|[<span data-ttu-id="623ae-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="623ae-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="623ae-143">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="623ae-143">Specifies the type of group policy.</span></span> <span data-ttu-id="623ae-144">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="623ae-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="623ae-145">firmware</span><span class="sxs-lookup"><span data-stu-id="623ae-145">revision</span></span>|<span data-ttu-id="623ae-146">String</span><span class="sxs-lookup"><span data-stu-id="623ae-146">String</span></span>|<span data-ttu-id="623ae-147">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="623ae-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="623ae-148">id</span><span class="sxs-lookup"><span data-stu-id="623ae-148">id</span></span>|<span data-ttu-id="623ae-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="623ae-149">String</span></span>|<span data-ttu-id="623ae-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="623ae-150">Key of the entity.</span></span>|
|<span data-ttu-id="623ae-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="623ae-151">lastModifiedDateTime</span></span>|<span data-ttu-id="623ae-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623ae-152">DateTimeOffset</span></span>|<span data-ttu-id="623ae-153">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="623ae-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="623ae-154">Relações</span><span class="sxs-lookup"><span data-stu-id="623ae-154">Relationships</span></span>
|<span data-ttu-id="623ae-155">Relação</span><span class="sxs-lookup"><span data-stu-id="623ae-155">Relationship</span></span>|<span data-ttu-id="623ae-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="623ae-156">Type</span></span>|<span data-ttu-id="623ae-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="623ae-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623ae-158">Definição</span><span class="sxs-lookup"><span data-stu-id="623ae-158">definitions</span></span>|<span data-ttu-id="623ae-159">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="623ae-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="623ae-160">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="623ae-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="623ae-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="623ae-161">JSON Representation</span></span>
<span data-ttu-id="623ae-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="623ae-162">Here is a JSON representation of the resource.</span></span>
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





