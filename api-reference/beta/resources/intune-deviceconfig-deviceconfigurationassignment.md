---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91181a787be06613302e618301ee8b8075bf41b6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725887"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="c6e52-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="c6e52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6e52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6e52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6e52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6e52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6e52-107">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="c6e52-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c6e52-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c6e52-108">Methods</span></span>
|<span data-ttu-id="c6e52-109">Método</span><span class="sxs-lookup"><span data-stu-id="c6e52-109">Method</span></span>|<span data-ttu-id="c6e52-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6e52-110">Return Type</span></span>|<span data-ttu-id="c6e52-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6e52-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6e52-112">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c6e52-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="c6e52-113">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6e52-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c6e52-114">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6e52-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c6e52-115">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="c6e52-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c6e52-117">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6e52-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c6e52-118">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="c6e52-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c6e52-120">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6e52-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c6e52-121">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="c6e52-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6e52-122">None</span></span>|<span data-ttu-id="c6e52-123">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6e52-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c6e52-124">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="c6e52-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6e52-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c6e52-126">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c6e52-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6e52-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6e52-127">Properties</span></span>
|<span data-ttu-id="c6e52-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6e52-128">Property</span></span>|<span data-ttu-id="c6e52-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6e52-129">Type</span></span>|<span data-ttu-id="c6e52-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6e52-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e52-131">id</span><span class="sxs-lookup"><span data-stu-id="c6e52-131">id</span></span>|<span data-ttu-id="c6e52-132">String</span><span class="sxs-lookup"><span data-stu-id="c6e52-132">String</span></span>|<span data-ttu-id="c6e52-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c6e52-133">The key of the assignment.</span></span>|
|<span data-ttu-id="c6e52-134">destino</span><span class="sxs-lookup"><span data-stu-id="c6e52-134">target</span></span>|[<span data-ttu-id="c6e52-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c6e52-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c6e52-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6e52-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="c6e52-137">source</span><span class="sxs-lookup"><span data-stu-id="c6e52-137">source</span></span>|[<span data-ttu-id="c6e52-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="c6e52-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="c6e52-139">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="c6e52-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="c6e52-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6e52-140">This property is read-only.</span></span> <span data-ttu-id="c6e52-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="c6e52-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="c6e52-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="c6e52-142">sourceId</span></span>|<span data-ttu-id="c6e52-143">String</span><span class="sxs-lookup"><span data-stu-id="c6e52-143">String</span></span>|<span data-ttu-id="c6e52-144">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c6e52-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="c6e52-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6e52-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6e52-146">Relações</span><span class="sxs-lookup"><span data-stu-id="c6e52-146">Relationships</span></span>
<span data-ttu-id="c6e52-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6e52-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6e52-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6e52-148">JSON Representation</span></span>
<span data-ttu-id="c6e52-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6e52-149">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```





