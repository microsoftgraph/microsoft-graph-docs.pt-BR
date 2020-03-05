---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5624f86622b49d8739de85a2c58067dd7263aace
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528111"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="0c3c3-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-103">groupPolicyConfiguration resource type</span></span>

<span data-ttu-id="0c3c3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c3c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c3c3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c3c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3c3-107">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="0c3c3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c3c3-108">Methods</span></span>
|<span data-ttu-id="0c3c3-109">Método</span><span class="sxs-lookup"><span data-stu-id="0c3c3-109">Method</span></span>|<span data-ttu-id="0c3c3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c3c3-110">Return Type</span></span>|<span data-ttu-id="0c3c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3c3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c3c3-112">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="0c3c3-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="0c3c3-113">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c3c3-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="0c3c3-114">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c3c3-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0c3c3-115">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="0c3c3-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0c3c3-117">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c3c3-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c3c3-118">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="0c3c3-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0c3c3-120">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c3c3-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c3c3-121">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="0c3c3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c3c3-122">None</span></span>|<span data-ttu-id="0c3c3-123">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c3c3-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="0c3c3-124">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="0c3c3-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c3c3-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="0c3c3-126">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c3c3-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c3c3-127">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="0c3c3-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="0c3c3-128">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0c3c3-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c3c3-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c3c3-129">Not yet documented</span></span>|
|[<span data-ttu-id="0c3c3-130">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="0c3c3-130">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="0c3c3-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0c3c3-131">None</span></span>|<span data-ttu-id="0c3c3-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c3c3-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0c3c3-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c3c3-133">Properties</span></span>
|<span data-ttu-id="0c3c3-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c3c3-134">Property</span></span>|<span data-ttu-id="0c3c3-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c3c3-135">Type</span></span>|<span data-ttu-id="0c3c3-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3c3-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3c3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c3c3-137">createdDateTime</span></span>|<span data-ttu-id="0c3c3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c3c3-138">DateTimeOffset</span></span>|<span data-ttu-id="0c3c3-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-139">The date and time the object was created.</span></span>|
|<span data-ttu-id="0c3c3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0c3c3-140">displayName</span></span>|<span data-ttu-id="0c3c3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c3c3-141">String</span></span>|<span data-ttu-id="0c3c3-142">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-142">User provided name for the resource object.</span></span>|
|<span data-ttu-id="0c3c3-143">description</span><span class="sxs-lookup"><span data-stu-id="0c3c3-143">description</span></span>|<span data-ttu-id="0c3c3-144">String</span><span class="sxs-lookup"><span data-stu-id="0c3c3-144">String</span></span>|<span data-ttu-id="0c3c3-145">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-145">User provided description for the resource object.</span></span>|
|<span data-ttu-id="0c3c3-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c3c3-146">roleScopeTagIds</span></span>|<span data-ttu-id="0c3c3-147">String collection</span><span class="sxs-lookup"><span data-stu-id="0c3c3-147">String collection</span></span>|<span data-ttu-id="0c3c3-148">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-148">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="0c3c3-149">id</span><span class="sxs-lookup"><span data-stu-id="0c3c3-149">id</span></span>|<span data-ttu-id="0c3c3-150">String</span><span class="sxs-lookup"><span data-stu-id="0c3c3-150">String</span></span>|<span data-ttu-id="0c3c3-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-151">Key of the entity.</span></span>|
|<span data-ttu-id="0c3c3-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c3c3-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0c3c3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c3c3-153">DateTimeOffset</span></span>|<span data-ttu-id="0c3c3-154">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c3c3-155">Relações</span><span class="sxs-lookup"><span data-stu-id="0c3c3-155">Relationships</span></span>
|<span data-ttu-id="0c3c3-156">Relação</span><span class="sxs-lookup"><span data-stu-id="0c3c3-156">Relationship</span></span>|<span data-ttu-id="0c3c3-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c3c3-157">Type</span></span>|<span data-ttu-id="0c3c3-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3c3-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3c3-159">definitionValues</span><span class="sxs-lookup"><span data-stu-id="0c3c3-159">definitionValues</span></span>|<span data-ttu-id="0c3c3-160">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0c3c3-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="0c3c3-161">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-161">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="0c3c3-162">assignments</span><span class="sxs-lookup"><span data-stu-id="0c3c3-162">assignments</span></span>|<span data-ttu-id="0c3c3-163">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0c3c3-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c3c3-164">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-164">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c3c3-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c3c3-165">JSON Representation</span></span>
<span data-ttu-id="0c3c3-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c3c3-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



