---
title: tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0ec4346174bdaafbc37c0721462ba8fd612abcc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975942"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="5cf19-103">tipo de recurso groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="5cf19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cf19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cf19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cf19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cf19-106">A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.</span><span class="sxs-lookup"><span data-stu-id="5cf19-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5cf19-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5cf19-107">Methods</span></span>
|<span data-ttu-id="5cf19-108">Método</span><span class="sxs-lookup"><span data-stu-id="5cf19-108">Method</span></span>|<span data-ttu-id="5cf19-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5cf19-109">Return Type</span></span>|<span data-ttu-id="5cf19-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf19-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5cf19-111">Listar groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="5cf19-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="5cf19-112">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5cf19-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5cf19-113">Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf19-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="5cf19-114">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="5cf19-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="5cf19-116">Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf19-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5cf19-117">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="5cf19-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="5cf19-119">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf19-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5cf19-120">Excluir groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="5cf19-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cf19-121">None</span></span>|<span data-ttu-id="5cf19-122">Exclui [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5cf19-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="5cf19-123">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="5cf19-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5cf19-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="5cf19-125">Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf19-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5cf19-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cf19-126">Properties</span></span>
|<span data-ttu-id="5cf19-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cf19-127">Property</span></span>|<span data-ttu-id="5cf19-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cf19-128">Type</span></span>|<span data-ttu-id="5cf19-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf19-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf19-130">id</span><span class="sxs-lookup"><span data-stu-id="5cf19-130">id</span></span>|<span data-ttu-id="5cf19-131">String</span><span class="sxs-lookup"><span data-stu-id="5cf19-131">String</span></span>|<span data-ttu-id="5cf19-132">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5cf19-132">Key of the entity.</span></span>|
|<span data-ttu-id="5cf19-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf19-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5cf19-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf19-134">DateTimeOffset</span></span>|<span data-ttu-id="5cf19-135">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5cf19-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="5cf19-136">destino</span><span class="sxs-lookup"><span data-stu-id="5cf19-136">target</span></span>|[<span data-ttu-id="5cf19-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5cf19-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5cf19-138">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="5cf19-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cf19-139">Relações</span><span class="sxs-lookup"><span data-stu-id="5cf19-139">Relationships</span></span>
<span data-ttu-id="5cf19-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cf19-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cf19-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cf19-141">JSON Representation</span></span>
<span data-ttu-id="5cf19-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cf19-142">Here is a JSON representation of the resource.</span></span>
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





