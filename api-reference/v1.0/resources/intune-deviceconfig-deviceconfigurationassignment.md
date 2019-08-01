---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcd13ad7884e572f60f642c087a30bada7dad7f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031672"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="13d1f-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="13d1f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13d1f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13d1f-105">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="13d1f-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="13d1f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="13d1f-106">Methods</span></span>
|<span data-ttu-id="13d1f-107">Método</span><span class="sxs-lookup"><span data-stu-id="13d1f-107">Method</span></span>|<span data-ttu-id="13d1f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13d1f-108">Return Type</span></span>|<span data-ttu-id="13d1f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d1f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13d1f-110">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="13d1f-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="13d1f-111">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="13d1f-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="13d1f-112">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="13d1f-113">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="13d1f-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="13d1f-115">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="13d1f-116">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="13d1f-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="13d1f-118">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="13d1f-119">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="13d1f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13d1f-120">None</span></span>|<span data-ttu-id="13d1f-121">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="13d1f-122">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="13d1f-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13d1f-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="13d1f-124">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13d1f-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13d1f-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13d1f-125">Properties</span></span>
|<span data-ttu-id="13d1f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13d1f-126">Property</span></span>|<span data-ttu-id="13d1f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d1f-127">Type</span></span>|<span data-ttu-id="13d1f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d1f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13d1f-129">id</span><span class="sxs-lookup"><span data-stu-id="13d1f-129">id</span></span>|<span data-ttu-id="13d1f-130">String</span><span class="sxs-lookup"><span data-stu-id="13d1f-130">String</span></span>|<span data-ttu-id="13d1f-131">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="13d1f-131">The key of the assignment.</span></span>|
|<span data-ttu-id="13d1f-132">destino</span><span class="sxs-lookup"><span data-stu-id="13d1f-132">target</span></span>|[<span data-ttu-id="13d1f-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="13d1f-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="13d1f-134">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13d1f-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13d1f-135">Relações</span><span class="sxs-lookup"><span data-stu-id="13d1f-135">Relationships</span></span>
<span data-ttu-id="13d1f-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13d1f-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13d1f-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13d1f-137">JSON Representation</span></span>
<span data-ttu-id="13d1f-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13d1f-138">Here is a JSON representation of the resource.</span></span>
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



