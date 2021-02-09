---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd2dad2bfb846a876e369a3b8fc1a36c846a8276
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154870"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="de42e-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="de42e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de42e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de42e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de42e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de42e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de42e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de42e-107">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="de42e-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="de42e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="de42e-108">Methods</span></span>
|<span data-ttu-id="de42e-109">Método</span><span class="sxs-lookup"><span data-stu-id="de42e-109">Method</span></span>|<span data-ttu-id="de42e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de42e-110">Return Type</span></span>|<span data-ttu-id="de42e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="de42e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de42e-112">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="de42e-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="de42e-113">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de42e-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="de42e-114">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de42e-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="de42e-115">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="de42e-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="de42e-117">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de42e-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="de42e-118">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="de42e-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="de42e-120">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de42e-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="de42e-121">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="de42e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de42e-122">None</span></span>|<span data-ttu-id="de42e-123">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de42e-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="de42e-124">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="de42e-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de42e-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="de42e-126">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de42e-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de42e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de42e-127">Properties</span></span>
|<span data-ttu-id="de42e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de42e-128">Property</span></span>|<span data-ttu-id="de42e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="de42e-129">Type</span></span>|<span data-ttu-id="de42e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="de42e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de42e-131">id</span><span class="sxs-lookup"><span data-stu-id="de42e-131">id</span></span>|<span data-ttu-id="de42e-132">String</span><span class="sxs-lookup"><span data-stu-id="de42e-132">String</span></span>|<span data-ttu-id="de42e-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="de42e-133">The key of the assignment.</span></span>|
|<span data-ttu-id="de42e-134">destino</span><span class="sxs-lookup"><span data-stu-id="de42e-134">target</span></span>|[<span data-ttu-id="de42e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de42e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de42e-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de42e-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="de42e-137">source</span><span class="sxs-lookup"><span data-stu-id="de42e-137">source</span></span>|[<span data-ttu-id="de42e-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="de42e-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="de42e-139">A origem da atribuição para a configuração do dispositivo, direta ou direta/policySet.</span><span class="sxs-lookup"><span data-stu-id="de42e-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="de42e-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de42e-140">This property is read-only.</span></span> <span data-ttu-id="de42e-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="de42e-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="de42e-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="de42e-142">sourceId</span></span>|<span data-ttu-id="de42e-143">String</span><span class="sxs-lookup"><span data-stu-id="de42e-143">String</span></span>|<span data-ttu-id="de42e-144">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="de42e-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="de42e-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de42e-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de42e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="de42e-146">Relationships</span></span>
<span data-ttu-id="de42e-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de42e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de42e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de42e-148">JSON Representation</span></span>
<span data-ttu-id="de42e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de42e-149">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




