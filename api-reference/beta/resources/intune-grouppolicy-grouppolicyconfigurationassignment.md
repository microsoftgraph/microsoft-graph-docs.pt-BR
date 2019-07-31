---
title: tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fc8b21bcf59eccee9460f1f39e3353d0a14bfaf4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998671"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="b0f59-103">tipo de recurso groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="b0f59-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0f59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0f59-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0f59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0f59-106">A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.</span><span class="sxs-lookup"><span data-stu-id="b0f59-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="b0f59-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0f59-107">Methods</span></span>
|<span data-ttu-id="b0f59-108">Método</span><span class="sxs-lookup"><span data-stu-id="b0f59-108">Method</span></span>|<span data-ttu-id="b0f59-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0f59-109">Return Type</span></span>|<span data-ttu-id="b0f59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0f59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0f59-111">Listar groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="b0f59-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="b0f59-112">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b0f59-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b0f59-113">Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f59-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="b0f59-114">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="b0f59-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f59-116">Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f59-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b0f59-117">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="b0f59-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f59-119">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f59-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b0f59-120">Excluir groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="b0f59-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0f59-121">None</span></span>|<span data-ttu-id="b0f59-122">Exclui [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b0f59-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="b0f59-123">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="b0f59-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f59-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f59-125">Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f59-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0f59-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0f59-126">Properties</span></span>
|<span data-ttu-id="b0f59-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0f59-127">Property</span></span>|<span data-ttu-id="b0f59-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0f59-128">Type</span></span>|<span data-ttu-id="b0f59-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0f59-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f59-130">id</span><span class="sxs-lookup"><span data-stu-id="b0f59-130">id</span></span>|<span data-ttu-id="b0f59-131">String</span><span class="sxs-lookup"><span data-stu-id="b0f59-131">String</span></span>|<span data-ttu-id="b0f59-132">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0f59-132">Key of the entity.</span></span>|
|<span data-ttu-id="b0f59-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f59-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b0f59-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0f59-134">DateTimeOffset</span></span>|<span data-ttu-id="b0f59-135">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0f59-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="b0f59-136">destino</span><span class="sxs-lookup"><span data-stu-id="b0f59-136">target</span></span>|[<span data-ttu-id="b0f59-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0f59-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b0f59-138">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="b0f59-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0f59-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b0f59-139">Relationships</span></span>
<span data-ttu-id="b0f59-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0f59-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0f59-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0f59-141">JSON Representation</span></span>
<span data-ttu-id="b0f59-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0f59-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





