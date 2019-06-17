---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a872671186e55524002b2d0a5f85b2ce1bbf2466
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975935"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="83e7a-105">tipo de recurso groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="83e7a-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="83e7a-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83e7a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83e7a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83e7a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83e7a-108">A entidade representa um arquivo XML ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="83e7a-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="83e7a-109">O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="83e7a-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="83e7a-110">O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.</span><span class="sxs-lookup"><span data-stu-id="83e7a-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="83e7a-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="83e7a-111">Methods</span></span>
|<span data-ttu-id="83e7a-112">Método</span><span class="sxs-lookup"><span data-stu-id="83e7a-112">Method</span></span>|<span data-ttu-id="83e7a-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83e7a-113">Return Type</span></span>|<span data-ttu-id="83e7a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="83e7a-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83e7a-115">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="83e7a-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="83e7a-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="83e7a-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="83e7a-117">Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="83e7a-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="83e7a-118">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="83e7a-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="83e7a-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="83e7a-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="83e7a-120">Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="83e7a-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83e7a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83e7a-121">Properties</span></span>
|<span data-ttu-id="83e7a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83e7a-122">Property</span></span>|<span data-ttu-id="83e7a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="83e7a-123">Type</span></span>|<span data-ttu-id="83e7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="83e7a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e7a-125">displayName</span><span class="sxs-lookup"><span data-stu-id="83e7a-125">displayName</span></span>|<span data-ttu-id="83e7a-126">String</span><span class="sxs-lookup"><span data-stu-id="83e7a-126">String</span></span>|<span data-ttu-id="83e7a-127">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="83e7a-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="83e7a-128">descrição</span><span class="sxs-lookup"><span data-stu-id="83e7a-128">description</span></span>|<span data-ttu-id="83e7a-129">String</span><span class="sxs-lookup"><span data-stu-id="83e7a-129">String</span></span>|<span data-ttu-id="83e7a-130">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="83e7a-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="83e7a-131">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="83e7a-131">The default value is empty.</span></span>|
|<span data-ttu-id="83e7a-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="83e7a-132">languageCodes</span></span>|<span data-ttu-id="83e7a-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83e7a-133">String collection</span></span>|<span data-ttu-id="83e7a-134">Os códigos de idioma suportados para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="83e7a-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="83e7a-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="83e7a-135">targetPrefix</span></span>|<span data-ttu-id="83e7a-136">String</span><span class="sxs-lookup"><span data-stu-id="83e7a-136">String</span></span>|<span data-ttu-id="83e7a-137">Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="83e7a-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="83e7a-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="83e7a-138">targetNamespace</span></span>|<span data-ttu-id="83e7a-139">String</span><span class="sxs-lookup"><span data-stu-id="83e7a-139">String</span></span>|<span data-ttu-id="83e7a-140">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="83e7a-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="83e7a-141">PolicyType</span><span class="sxs-lookup"><span data-stu-id="83e7a-141">policyType</span></span>|[<span data-ttu-id="83e7a-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="83e7a-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="83e7a-143">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="83e7a-143">Specifies the type of group policy.</span></span> <span data-ttu-id="83e7a-144">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="83e7a-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="83e7a-145">id</span><span class="sxs-lookup"><span data-stu-id="83e7a-145">id</span></span>|<span data-ttu-id="83e7a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83e7a-146">String</span></span>|<span data-ttu-id="83e7a-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83e7a-147">Key of the entity.</span></span>|
|<span data-ttu-id="83e7a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83e7a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="83e7a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83e7a-149">DateTimeOffset</span></span>|<span data-ttu-id="83e7a-150">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="83e7a-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83e7a-151">Relações</span><span class="sxs-lookup"><span data-stu-id="83e7a-151">Relationships</span></span>
|<span data-ttu-id="83e7a-152">Relação</span><span class="sxs-lookup"><span data-stu-id="83e7a-152">Relationship</span></span>|<span data-ttu-id="83e7a-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="83e7a-153">Type</span></span>|<span data-ttu-id="83e7a-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="83e7a-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e7a-155">Definição</span><span class="sxs-lookup"><span data-stu-id="83e7a-155">definitions</span></span>|<span data-ttu-id="83e7a-156">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="83e7a-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="83e7a-157">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="83e7a-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83e7a-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83e7a-158">JSON Representation</span></span>
<span data-ttu-id="83e7a-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83e7a-159">Here is a JSON representation of the resource.</span></span>
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





