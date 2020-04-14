---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e2d017b7bbd8f76d59f7862fbb943c455c78fbe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377077"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="d8bff-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-103">groupPolicyConfiguration resource type</span></span>

<span data-ttu-id="d8bff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8bff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8bff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8bff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8bff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8bff-107">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="d8bff-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="d8bff-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8bff-108">Methods</span></span>
|<span data-ttu-id="d8bff-109">Método</span><span class="sxs-lookup"><span data-stu-id="d8bff-109">Method</span></span>|<span data-ttu-id="d8bff-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8bff-110">Return Type</span></span>|<span data-ttu-id="d8bff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8bff-112">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="d8bff-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="d8bff-113">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8bff-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="d8bff-114">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bff-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d8bff-115">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="d8bff-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d8bff-117">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bff-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8bff-118">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="d8bff-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d8bff-120">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bff-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8bff-121">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="d8bff-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8bff-122">None</span></span>|<span data-ttu-id="d8bff-123">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8bff-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="d8bff-124">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="d8bff-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8bff-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d8bff-126">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bff-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d8bff-127">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d8bff-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="d8bff-128">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d8bff-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d8bff-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d8bff-129">Not yet documented</span></span>|
|[<span data-ttu-id="d8bff-130">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="d8bff-130">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="d8bff-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d8bff-131">None</span></span>|<span data-ttu-id="d8bff-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d8bff-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d8bff-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8bff-133">Properties</span></span>
|<span data-ttu-id="d8bff-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8bff-134">Property</span></span>|<span data-ttu-id="d8bff-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bff-135">Type</span></span>|<span data-ttu-id="d8bff-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bff-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bff-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8bff-137">createdDateTime</span></span>|<span data-ttu-id="d8bff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8bff-138">DateTimeOffset</span></span>|<span data-ttu-id="d8bff-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d8bff-139">The date and time the object was created.</span></span>|
|<span data-ttu-id="d8bff-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d8bff-140">displayName</span></span>|<span data-ttu-id="d8bff-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8bff-141">String</span></span>|<span data-ttu-id="d8bff-142">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="d8bff-142">User provided name for the resource object.</span></span>|
|<span data-ttu-id="d8bff-143">description</span><span class="sxs-lookup"><span data-stu-id="d8bff-143">description</span></span>|<span data-ttu-id="d8bff-144">String</span><span class="sxs-lookup"><span data-stu-id="d8bff-144">String</span></span>|<span data-ttu-id="d8bff-145">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="d8bff-145">User provided description for the resource object.</span></span>|
|<span data-ttu-id="d8bff-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8bff-146">roleScopeTagIds</span></span>|<span data-ttu-id="d8bff-147">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d8bff-147">String collection</span></span>|<span data-ttu-id="d8bff-148">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d8bff-148">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="d8bff-149">id</span><span class="sxs-lookup"><span data-stu-id="d8bff-149">id</span></span>|<span data-ttu-id="d8bff-150">String</span><span class="sxs-lookup"><span data-stu-id="d8bff-150">String</span></span>|<span data-ttu-id="d8bff-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8bff-151">Key of the entity.</span></span>|
|<span data-ttu-id="d8bff-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8bff-152">lastModifiedDateTime</span></span>|<span data-ttu-id="d8bff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8bff-153">DateTimeOffset</span></span>|<span data-ttu-id="d8bff-154">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d8bff-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8bff-155">Relações</span><span class="sxs-lookup"><span data-stu-id="d8bff-155">Relationships</span></span>
|<span data-ttu-id="d8bff-156">Relação</span><span class="sxs-lookup"><span data-stu-id="d8bff-156">Relationship</span></span>|<span data-ttu-id="d8bff-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bff-157">Type</span></span>|<span data-ttu-id="d8bff-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bff-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bff-159">definitionValues</span><span class="sxs-lookup"><span data-stu-id="d8bff-159">definitionValues</span></span>|<span data-ttu-id="d8bff-160">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d8bff-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="d8bff-161">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d8bff-161">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="d8bff-162">assignments</span><span class="sxs-lookup"><span data-stu-id="d8bff-162">assignments</span></span>|<span data-ttu-id="d8bff-163">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d8bff-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d8bff-164">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d8bff-164">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8bff-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8bff-165">JSON Representation</span></span>
<span data-ttu-id="d8bff-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8bff-166">Here is a JSON representation of the resource.</span></span>
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



