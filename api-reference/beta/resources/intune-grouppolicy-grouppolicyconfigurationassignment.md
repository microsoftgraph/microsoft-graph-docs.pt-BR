---
title: tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcc3b313ca13c830c4924fa73b1ae09537069301
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793875"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="c845d-103">tipo de recurso groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="c845d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c845d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c845d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c845d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c845d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c845d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c845d-107">A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.</span><span class="sxs-lookup"><span data-stu-id="c845d-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c845d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="c845d-108">Methods</span></span>
|<span data-ttu-id="c845d-109">Método</span><span class="sxs-lookup"><span data-stu-id="c845d-109">Method</span></span>|<span data-ttu-id="c845d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c845d-110">Return Type</span></span>|<span data-ttu-id="c845d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c845d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c845d-112">Listar groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c845d-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="c845d-113">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c845d-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c845d-114">Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c845d-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c845d-115">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="c845d-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c845d-117">Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c845d-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c845d-118">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="c845d-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c845d-120">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c845d-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c845d-121">Excluir groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="c845d-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c845d-122">None</span></span>|<span data-ttu-id="c845d-123">Exclui [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c845d-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c845d-124">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="c845d-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c845d-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c845d-126">Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c845d-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c845d-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c845d-127">Properties</span></span>
|<span data-ttu-id="c845d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c845d-128">Property</span></span>|<span data-ttu-id="c845d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c845d-129">Type</span></span>|<span data-ttu-id="c845d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c845d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c845d-131">id</span><span class="sxs-lookup"><span data-stu-id="c845d-131">id</span></span>|<span data-ttu-id="c845d-132">String</span><span class="sxs-lookup"><span data-stu-id="c845d-132">String</span></span>|<span data-ttu-id="c845d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c845d-133">Key of the entity.</span></span>|
|<span data-ttu-id="c845d-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c845d-134">lastModifiedDateTime</span></span>|<span data-ttu-id="c845d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c845d-135">DateTimeOffset</span></span>|<span data-ttu-id="c845d-136">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c845d-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c845d-137">destino</span><span class="sxs-lookup"><span data-stu-id="c845d-137">target</span></span>|[<span data-ttu-id="c845d-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c845d-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c845d-139">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="c845d-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c845d-140">Relações</span><span class="sxs-lookup"><span data-stu-id="c845d-140">Relationships</span></span>
<span data-ttu-id="c845d-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c845d-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c845d-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c845d-142">JSON Representation</span></span>
<span data-ttu-id="c845d-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c845d-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



