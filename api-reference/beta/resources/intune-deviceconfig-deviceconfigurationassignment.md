---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80645a7b6724a71620eeebf4dfb4ba8a1b440db2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172629"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="df67d-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="df67d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df67d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df67d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df67d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df67d-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="df67d-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="df67d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="df67d-107">Methods</span></span>
|<span data-ttu-id="df67d-108">Método</span><span class="sxs-lookup"><span data-stu-id="df67d-108">Method</span></span>|<span data-ttu-id="df67d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="df67d-109">Return Type</span></span>|<span data-ttu-id="df67d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df67d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df67d-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="df67d-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="df67d-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="df67d-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="df67d-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df67d-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="df67d-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="df67d-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df67d-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df67d-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="df67d-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="df67d-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df67d-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df67d-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="df67d-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="df67d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df67d-121">None</span></span>|<span data-ttu-id="df67d-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df67d-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="df67d-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="df67d-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df67d-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df67d-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df67d-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df67d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df67d-126">Properties</span></span>
|<span data-ttu-id="df67d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df67d-127">Property</span></span>|<span data-ttu-id="df67d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="df67d-128">Type</span></span>|<span data-ttu-id="df67d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="df67d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df67d-130">id</span><span class="sxs-lookup"><span data-stu-id="df67d-130">id</span></span>|<span data-ttu-id="df67d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df67d-131">String</span></span>|<span data-ttu-id="df67d-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="df67d-132">The key of the assignment.</span></span>|
|<span data-ttu-id="df67d-133">destino</span><span class="sxs-lookup"><span data-stu-id="df67d-133">target</span></span>|[<span data-ttu-id="df67d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="df67d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="df67d-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df67d-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df67d-136">Relações</span><span class="sxs-lookup"><span data-stu-id="df67d-136">Relationships</span></span>
<span data-ttu-id="df67d-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="df67d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df67d-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df67d-138">JSON Representation</span></span>
<span data-ttu-id="df67d-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df67d-139">Here is a JSON representation of the resource.</span></span>
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
  }
}
```




