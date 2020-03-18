---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f86b85cd63c619e5ee5447e3f19a66f2a6524767
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793279"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="8cb83-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="8cb83-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cb83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cb83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cb83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb83-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="8cb83-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8cb83-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8cb83-107">Methods</span></span>
|<span data-ttu-id="8cb83-108">Método</span><span class="sxs-lookup"><span data-stu-id="8cb83-108">Method</span></span>|<span data-ttu-id="8cb83-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8cb83-109">Return Type</span></span>|<span data-ttu-id="8cb83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb83-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8cb83-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8cb83-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="8cb83-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8cb83-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8cb83-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8cb83-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="8cb83-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="8cb83-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8cb83-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8cb83-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8cb83-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="8cb83-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8cb83-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8cb83-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8cb83-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="8cb83-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cb83-121">None</span></span>|<span data-ttu-id="8cb83-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8cb83-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="8cb83-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="8cb83-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb83-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8cb83-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8cb83-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cb83-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cb83-126">Properties</span></span>
|<span data-ttu-id="8cb83-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cb83-127">Property</span></span>|<span data-ttu-id="8cb83-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb83-128">Type</span></span>|<span data-ttu-id="8cb83-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb83-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb83-130">id</span><span class="sxs-lookup"><span data-stu-id="8cb83-130">id</span></span>|<span data-ttu-id="8cb83-131">String</span><span class="sxs-lookup"><span data-stu-id="8cb83-131">String</span></span>|<span data-ttu-id="8cb83-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8cb83-132">The key of the assignment.</span></span>|
|<span data-ttu-id="8cb83-133">destino</span><span class="sxs-lookup"><span data-stu-id="8cb83-133">target</span></span>|[<span data-ttu-id="8cb83-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8cb83-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8cb83-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8cb83-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="8cb83-136">source</span><span class="sxs-lookup"><span data-stu-id="8cb83-136">source</span></span>|[<span data-ttu-id="8cb83-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8cb83-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8cb83-138">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="8cb83-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="8cb83-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8cb83-139">This property is read-only.</span></span> <span data-ttu-id="8cb83-140">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="8cb83-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8cb83-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="8cb83-141">sourceId</span></span>|<span data-ttu-id="8cb83-142">String</span><span class="sxs-lookup"><span data-stu-id="8cb83-142">String</span></span>|<span data-ttu-id="8cb83-143">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8cb83-143">The identifier of the source of the assignment.</span></span> <span data-ttu-id="8cb83-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8cb83-144">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cb83-145">Relações</span><span class="sxs-lookup"><span data-stu-id="8cb83-145">Relationships</span></span>
<span data-ttu-id="8cb83-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cb83-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cb83-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cb83-147">JSON Representation</span></span>
<span data-ttu-id="8cb83-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cb83-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



