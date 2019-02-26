---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540da94d92f3056a6699b7112f3589f6da4b7144
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160750"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="ec364-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="ec364-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec364-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec364-106">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="ec364-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="ec364-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec364-107">Methods</span></span>
|<span data-ttu-id="ec364-108">Método</span><span class="sxs-lookup"><span data-stu-id="ec364-108">Method</span></span>|<span data-ttu-id="ec364-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec364-109">Return Type</span></span>|<span data-ttu-id="ec364-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec364-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec364-111">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="ec364-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="ec364-112">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec364-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="ec364-113">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ec364-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ec364-114">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="ec364-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ec364-116">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ec364-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ec364-117">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="ec364-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ec364-119">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ec364-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ec364-120">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="ec364-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec364-121">None</span></span>|<span data-ttu-id="ec364-122">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec364-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="ec364-123">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="ec364-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec364-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ec364-125">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ec364-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ec364-126">Ação assign</span><span class="sxs-lookup"><span data-stu-id="ec364-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="ec364-127">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec364-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ec364-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ec364-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ec364-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec364-129">Properties</span></span>
|<span data-ttu-id="ec364-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec364-130">Property</span></span>|<span data-ttu-id="ec364-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec364-131">Type</span></span>|<span data-ttu-id="ec364-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec364-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec364-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec364-133">createdDateTime</span></span>|<span data-ttu-id="ec364-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec364-134">DateTimeOffset</span></span>|<span data-ttu-id="ec364-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ec364-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="ec364-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ec364-136">displayName</span></span>|<span data-ttu-id="ec364-137">String</span><span class="sxs-lookup"><span data-stu-id="ec364-137">String</span></span>|<span data-ttu-id="ec364-138">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="ec364-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="ec364-139">description</span><span class="sxs-lookup"><span data-stu-id="ec364-139">description</span></span>|<span data-ttu-id="ec364-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec364-140">String</span></span>|<span data-ttu-id="ec364-141">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="ec364-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="ec364-142">id</span><span class="sxs-lookup"><span data-stu-id="ec364-142">id</span></span>|<span data-ttu-id="ec364-143">String</span><span class="sxs-lookup"><span data-stu-id="ec364-143">String</span></span>|<span data-ttu-id="ec364-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec364-144">Key of the entity.</span></span>|
|<span data-ttu-id="ec364-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec364-145">lastModifiedDateTime</span></span>|<span data-ttu-id="ec364-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec364-146">DateTimeOffset</span></span>|<span data-ttu-id="ec364-147">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ec364-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec364-148">Relações</span><span class="sxs-lookup"><span data-stu-id="ec364-148">Relationships</span></span>
|<span data-ttu-id="ec364-149">Relação</span><span class="sxs-lookup"><span data-stu-id="ec364-149">Relationship</span></span>|<span data-ttu-id="ec364-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec364-150">Type</span></span>|<span data-ttu-id="ec364-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec364-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec364-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="ec364-152">definitionValues</span></span>|<span data-ttu-id="ec364-153">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ec364-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="ec364-154">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="ec364-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="ec364-155">assignments</span><span class="sxs-lookup"><span data-stu-id="ec364-155">assignments</span></span>|<span data-ttu-id="ec364-156">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ec364-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ec364-157">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="ec364-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec364-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec364-158">JSON Representation</span></span>
<span data-ttu-id="ec364-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec364-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




