---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e344554804044687c7e5b9aa90c6171055b64a16
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37198191"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="21dd2-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="21dd2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21dd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21dd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21dd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21dd2-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="21dd2-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="21dd2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="21dd2-107">Methods</span></span>
|<span data-ttu-id="21dd2-108">Método</span><span class="sxs-lookup"><span data-stu-id="21dd2-108">Method</span></span>|<span data-ttu-id="21dd2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21dd2-109">Return Type</span></span>|<span data-ttu-id="21dd2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21dd2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21dd2-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="21dd2-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="21dd2-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="21dd2-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="21dd2-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dd2-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="21dd2-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="21dd2-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="21dd2-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dd2-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="21dd2-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="21dd2-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="21dd2-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dd2-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="21dd2-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="21dd2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21dd2-121">None</span></span>|<span data-ttu-id="21dd2-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dd2-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="21dd2-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="21dd2-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="21dd2-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="21dd2-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21dd2-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21dd2-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21dd2-126">Properties</span></span>
|<span data-ttu-id="21dd2-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21dd2-127">Property</span></span>|<span data-ttu-id="21dd2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="21dd2-128">Type</span></span>|<span data-ttu-id="21dd2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="21dd2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21dd2-130">id</span><span class="sxs-lookup"><span data-stu-id="21dd2-130">id</span></span>|<span data-ttu-id="21dd2-131">String</span><span class="sxs-lookup"><span data-stu-id="21dd2-131">String</span></span>|<span data-ttu-id="21dd2-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="21dd2-132">The key of the assignment.</span></span>|
|<span data-ttu-id="21dd2-133">destino</span><span class="sxs-lookup"><span data-stu-id="21dd2-133">target</span></span>|[<span data-ttu-id="21dd2-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21dd2-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="21dd2-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21dd2-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="21dd2-136">source</span><span class="sxs-lookup"><span data-stu-id="21dd2-136">source</span></span>|[<span data-ttu-id="21dd2-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="21dd2-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="21dd2-138">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="21dd2-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="21dd2-139">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="21dd2-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="21dd2-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="21dd2-140">sourceId</span></span>|<span data-ttu-id="21dd2-141">String</span><span class="sxs-lookup"><span data-stu-id="21dd2-141">String</span></span>|<span data-ttu-id="21dd2-142">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="21dd2-142">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21dd2-143">Relações</span><span class="sxs-lookup"><span data-stu-id="21dd2-143">Relationships</span></span>
<span data-ttu-id="21dd2-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21dd2-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21dd2-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21dd2-145">JSON Representation</span></span>
<span data-ttu-id="21dd2-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21dd2-146">Here is a JSON representation of the resource.</span></span>
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



