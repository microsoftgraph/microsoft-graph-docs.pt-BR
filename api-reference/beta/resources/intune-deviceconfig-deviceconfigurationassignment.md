---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3580454eae767f9a9ca84e3ab196d66fb0c363d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993162"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="c0a09-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="c0a09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0a09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0a09-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="c0a09-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c0a09-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0a09-107">Methods</span></span>
|<span data-ttu-id="c0a09-108">Método</span><span class="sxs-lookup"><span data-stu-id="c0a09-108">Method</span></span>|<span data-ttu-id="c0a09-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0a09-109">Return Type</span></span>|<span data-ttu-id="c0a09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0a09-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0a09-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c0a09-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="c0a09-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c0a09-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c0a09-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0a09-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c0a09-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="c0a09-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c0a09-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0a09-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c0a09-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="c0a09-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c0a09-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0a09-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c0a09-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="c0a09-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0a09-121">None</span></span>|<span data-ttu-id="c0a09-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0a09-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c0a09-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="c0a09-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0a09-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c0a09-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0a09-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0a09-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0a09-126">Properties</span></span>
|<span data-ttu-id="c0a09-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0a09-127">Property</span></span>|<span data-ttu-id="c0a09-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0a09-128">Type</span></span>|<span data-ttu-id="c0a09-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0a09-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0a09-130">id</span><span class="sxs-lookup"><span data-stu-id="c0a09-130">id</span></span>|<span data-ttu-id="c0a09-131">String</span><span class="sxs-lookup"><span data-stu-id="c0a09-131">String</span></span>|<span data-ttu-id="c0a09-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c0a09-132">The key of the assignment.</span></span>|
|<span data-ttu-id="c0a09-133">destino</span><span class="sxs-lookup"><span data-stu-id="c0a09-133">target</span></span>|[<span data-ttu-id="c0a09-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c0a09-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c0a09-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0a09-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0a09-136">Relações</span><span class="sxs-lookup"><span data-stu-id="c0a09-136">Relationships</span></span>
<span data-ttu-id="c0a09-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0a09-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0a09-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0a09-138">JSON Representation</span></span>
<span data-ttu-id="c0a09-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0a09-139">Here is a JSON representation of the resource.</span></span>
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





