---
title: tipo de recurso de groupPolicyDefinitionFile
description: A entidade representa um arquivo XML de ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus respectivos locais pelo caminho de categoria. O arquivo de definição de diretiva de grupo também contém os idiomas com suporte conforme determinado pelos arquivos de idioma ADML (Administrative Template) dependentes de idioma.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431261"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="c45af-105">tipo de recurso de groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c45af-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="c45af-106">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c45af-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c45af-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c45af-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c45af-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c45af-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c45af-109">A entidade representa um arquivo XML de ADMX (modelo administrativo).</span><span class="sxs-lookup"><span data-stu-id="c45af-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="c45af-110">O arquivo ADMX contém uma coleção de definições de política de grupo e seus respectivos locais pelo caminho de categoria.</span><span class="sxs-lookup"><span data-stu-id="c45af-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="c45af-111">O arquivo de definição de diretiva de grupo também contém os idiomas com suporte conforme determinado pelos arquivos de idioma ADML (Administrative Template) dependentes de idioma.</span><span class="sxs-lookup"><span data-stu-id="c45af-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="c45af-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="c45af-112">Methods</span></span>
|<span data-ttu-id="c45af-113">Método</span><span class="sxs-lookup"><span data-stu-id="c45af-113">Method</span></span>|<span data-ttu-id="c45af-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c45af-114">Return Type</span></span>|<span data-ttu-id="c45af-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45af-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c45af-116">Obter groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c45af-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="c45af-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c45af-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="c45af-118">Leia as propriedades e os relacionamentos do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="c45af-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="c45af-119">Atualizar groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c45af-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="c45af-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c45af-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="c45af-121">Atualize as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="c45af-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c45af-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c45af-122">Properties</span></span>
|<span data-ttu-id="c45af-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c45af-123">Property</span></span>|<span data-ttu-id="c45af-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c45af-124">Type</span></span>|<span data-ttu-id="c45af-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45af-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c45af-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c45af-126">displayName</span></span>|<span data-ttu-id="c45af-127">String</span><span class="sxs-lookup"><span data-stu-id="c45af-127">String</span></span>|<span data-ttu-id="c45af-128">O nome amigável localizado do arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c45af-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="c45af-129">description</span><span class="sxs-lookup"><span data-stu-id="c45af-129">description</span></span>|<span data-ttu-id="c45af-130">String</span><span class="sxs-lookup"><span data-stu-id="c45af-130">String</span></span>|<span data-ttu-id="c45af-131">A descrição localizada das configurações de política no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c45af-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="c45af-132">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="c45af-132">The default value is empty.</span></span>|
|<span data-ttu-id="c45af-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="c45af-133">languageCodes</span></span>|<span data-ttu-id="c45af-134">String collection</span><span class="sxs-lookup"><span data-stu-id="c45af-134">String collection</span></span>|<span data-ttu-id="c45af-135">Os códigos de idioma com suporte para o arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c45af-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="c45af-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="c45af-136">targetPrefix</span></span>|<span data-ttu-id="c45af-137">String</span><span class="sxs-lookup"><span data-stu-id="c45af-137">String</span></span>|<span data-ttu-id="c45af-138">Especifica o nome lógico que se refere ao namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c45af-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c45af-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="c45af-139">targetNamespace</span></span>|<span data-ttu-id="c45af-140">String</span><span class="sxs-lookup"><span data-stu-id="c45af-140">String</span></span>|<span data-ttu-id="c45af-141">Especifica o URI usado para identificar o namespace no arquivo ADMX.</span><span class="sxs-lookup"><span data-stu-id="c45af-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="c45af-142">policyType</span><span class="sxs-lookup"><span data-stu-id="c45af-142">policyType</span></span>|[<span data-ttu-id="c45af-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c45af-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c45af-144">Especifica o tipo de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="c45af-144">Specifies the type of group policy.</span></span> <span data-ttu-id="c45af-145">Os valores possíveis são: `admxBacked` e `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="c45af-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c45af-146">id</span><span class="sxs-lookup"><span data-stu-id="c45af-146">id</span></span>|<span data-ttu-id="c45af-147">String</span><span class="sxs-lookup"><span data-stu-id="c45af-147">String</span></span>|<span data-ttu-id="c45af-148">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c45af-148">Key of the entity.</span></span>|
|<span data-ttu-id="c45af-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c45af-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c45af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c45af-150">DateTimeOffset</span></span>|<span data-ttu-id="c45af-151">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c45af-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c45af-152">Relações</span><span class="sxs-lookup"><span data-stu-id="c45af-152">Relationships</span></span>
|<span data-ttu-id="c45af-153">Relação</span><span class="sxs-lookup"><span data-stu-id="c45af-153">Relationship</span></span>|<span data-ttu-id="c45af-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="c45af-154">Type</span></span>|<span data-ttu-id="c45af-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="c45af-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c45af-156">definições</span><span class="sxs-lookup"><span data-stu-id="c45af-156">definitions</span></span>|<span data-ttu-id="c45af-157">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c45af-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="c45af-158">As definições de política de grupo associadas ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="c45af-158">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c45af-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c45af-159">JSON Representation</span></span>
<span data-ttu-id="c45af-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c45af-160">Here is a JSON representation of the resource.</span></span>
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




