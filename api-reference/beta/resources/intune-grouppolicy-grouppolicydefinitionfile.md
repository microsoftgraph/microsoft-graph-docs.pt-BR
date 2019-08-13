---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98881f482f0feda24d070cd52c83d5de7dc5def9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331459"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="1b3fd-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="1b3fd-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="1b3fd-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b3fd-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b3fd-108">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="1b3fd-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="1b3fd-109">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="1b3fd-110">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="1b3fd-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b3fd-111">Methods</span></span>
|<span data-ttu-id="1b3fd-112">Método</span><span class="sxs-lookup"><span data-stu-id="1b3fd-112">Method</span></span>|<span data-ttu-id="1b3fd-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b3fd-113">Return Type</span></span>|<span data-ttu-id="1b3fd-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b3fd-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b3fd-115">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="1b3fd-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="1b3fd-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="1b3fd-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="1b3fd-117">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="1b3fd-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="1b3fd-118">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="1b3fd-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="1b3fd-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="1b3fd-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="1b3fd-120">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="1b3fd-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b3fd-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b3fd-121">Properties</span></span>
|<span data-ttu-id="1b3fd-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b3fd-122">Property</span></span>|<span data-ttu-id="1b3fd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b3fd-123">Type</span></span>|<span data-ttu-id="1b3fd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b3fd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3fd-125">displayName</span><span class="sxs-lookup"><span data-stu-id="1b3fd-125">displayName</span></span>|<span data-ttu-id="1b3fd-126">String</span><span class="sxs-lookup"><span data-stu-id="1b3fd-126">String</span></span>|<span data-ttu-id="1b3fd-127">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="1b3fd-128">descrição</span><span class="sxs-lookup"><span data-stu-id="1b3fd-128">description</span></span>|<span data-ttu-id="1b3fd-129">String</span><span class="sxs-lookup"><span data-stu-id="1b3fd-129">String</span></span>|<span data-ttu-id="1b3fd-130">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="1b3fd-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-131">The default value is empty.</span></span>|
|<span data-ttu-id="1b3fd-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="1b3fd-132">languageCodes</span></span>|<span data-ttu-id="1b3fd-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b3fd-133">String collection</span></span>|<span data-ttu-id="1b3fd-134">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="1b3fd-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="1b3fd-135">targetPrefix</span></span>|<span data-ttu-id="1b3fd-136">String</span><span class="sxs-lookup"><span data-stu-id="1b3fd-136">String</span></span>|<span data-ttu-id="1b3fd-137">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="1b3fd-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="1b3fd-138">targetNamespace</span></span>|<span data-ttu-id="1b3fd-139">String</span><span class="sxs-lookup"><span data-stu-id="1b3fd-139">String</span></span>|<span data-ttu-id="1b3fd-140">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="1b3fd-141">PolicyType</span><span class="sxs-lookup"><span data-stu-id="1b3fd-141">policyType</span></span>|[<span data-ttu-id="1b3fd-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="1b3fd-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="1b3fd-143">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-143">Specifies the type of group policy.</span></span> <span data-ttu-id="1b3fd-144">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="1b3fd-145">firmware</span><span class="sxs-lookup"><span data-stu-id="1b3fd-145">revision</span></span>|<span data-ttu-id="1b3fd-146">String</span><span class="sxs-lookup"><span data-stu-id="1b3fd-146">String</span></span>|<span data-ttu-id="1b3fd-147">A versão de revisão associada ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="1b3fd-148">id</span><span class="sxs-lookup"><span data-stu-id="1b3fd-148">id</span></span>|<span data-ttu-id="1b3fd-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b3fd-149">String</span></span>|<span data-ttu-id="1b3fd-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-150">Key of the entity.</span></span>|
|<span data-ttu-id="1b3fd-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b3fd-151">lastModifiedDateTime</span></span>|<span data-ttu-id="1b3fd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3fd-152">DateTimeOffset</span></span>|<span data-ttu-id="1b3fd-153">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b3fd-154">Relações</span><span class="sxs-lookup"><span data-stu-id="1b3fd-154">Relationships</span></span>
|<span data-ttu-id="1b3fd-155">Relação</span><span class="sxs-lookup"><span data-stu-id="1b3fd-155">Relationship</span></span>|<span data-ttu-id="1b3fd-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b3fd-156">Type</span></span>|<span data-ttu-id="1b3fd-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b3fd-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3fd-158">Definição</span><span class="sxs-lookup"><span data-stu-id="1b3fd-158">definitions</span></span>|<span data-ttu-id="1b3fd-159">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b3fd-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="1b3fd-160">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b3fd-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b3fd-161">JSON Representation</span></span>
<span data-ttu-id="1b3fd-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b3fd-162">Here is a JSON representation of the resource.</span></span>
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



