---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e75d4f76a37fc6497fe0c796f3cd22ac1eda40d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465731"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="2ab1b-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="2ab1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab1b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ab1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab1b-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="2ab1b-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2ab1b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ab1b-107">Methods</span></span>
|<span data-ttu-id="2ab1b-108">Método</span><span class="sxs-lookup"><span data-stu-id="2ab1b-108">Method</span></span>|<span data-ttu-id="2ab1b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ab1b-109">Return Type</span></span>|<span data-ttu-id="2ab1b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ab1b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ab1b-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="2ab1b-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="2ab1b-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2ab1b-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2ab1b-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1b-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2ab1b-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="2ab1b-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2ab1b-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1b-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2ab1b-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="2ab1b-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2ab1b-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1b-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2ab1b-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="2ab1b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ab1b-121">None</span></span>|<span data-ttu-id="2ab1b-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1b-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2ab1b-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="2ab1b-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ab1b-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2ab1b-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ab1b-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ab1b-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ab1b-126">Properties</span></span>
|<span data-ttu-id="2ab1b-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ab1b-127">Property</span></span>|<span data-ttu-id="2ab1b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ab1b-128">Type</span></span>|<span data-ttu-id="2ab1b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ab1b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab1b-130">id</span><span class="sxs-lookup"><span data-stu-id="2ab1b-130">id</span></span>|<span data-ttu-id="2ab1b-131">String</span><span class="sxs-lookup"><span data-stu-id="2ab1b-131">String</span></span>|<span data-ttu-id="2ab1b-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2ab1b-132">The key of the assignment.</span></span>|
|<span data-ttu-id="2ab1b-133">destino</span><span class="sxs-lookup"><span data-stu-id="2ab1b-133">target</span></span>|[<span data-ttu-id="2ab1b-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2ab1b-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2ab1b-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ab1b-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab1b-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2ab1b-136">Relationships</span></span>
<span data-ttu-id="2ab1b-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ab1b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ab1b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ab1b-138">JSON Representation</span></span>
<span data-ttu-id="2ab1b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ab1b-139">Here is a JSON representation of the resource.</span></span>
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







