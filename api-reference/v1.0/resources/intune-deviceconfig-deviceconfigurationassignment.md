---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fb4f0a782d9502f9e3da3f0a7da2389e937a7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573414"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="82d47-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="82d47-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82d47-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d47-105">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="82d47-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="82d47-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="82d47-106">Methods</span></span>
|<span data-ttu-id="82d47-107">Método</span><span class="sxs-lookup"><span data-stu-id="82d47-107">Method</span></span>|<span data-ttu-id="82d47-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82d47-108">Return Type</span></span>|<span data-ttu-id="82d47-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="82d47-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="82d47-110">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="82d47-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="82d47-111">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="82d47-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="82d47-112">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82d47-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="82d47-113">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="82d47-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="82d47-115">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82d47-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="82d47-116">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="82d47-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="82d47-118">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82d47-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="82d47-119">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="82d47-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82d47-120">None</span></span>|<span data-ttu-id="82d47-121">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82d47-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="82d47-122">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="82d47-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82d47-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="82d47-124">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82d47-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="82d47-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82d47-125">Properties</span></span>
|<span data-ttu-id="82d47-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82d47-126">Property</span></span>|<span data-ttu-id="82d47-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="82d47-127">Type</span></span>|<span data-ttu-id="82d47-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="82d47-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d47-129">id</span><span class="sxs-lookup"><span data-stu-id="82d47-129">id</span></span>|<span data-ttu-id="82d47-130">String</span><span class="sxs-lookup"><span data-stu-id="82d47-130">String</span></span>|<span data-ttu-id="82d47-131">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="82d47-131">The key of the assignment.</span></span>|
|<span data-ttu-id="82d47-132">destino</span><span class="sxs-lookup"><span data-stu-id="82d47-132">target</span></span>|[<span data-ttu-id="82d47-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82d47-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82d47-134">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82d47-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82d47-135">Relações</span><span class="sxs-lookup"><span data-stu-id="82d47-135">Relationships</span></span>
<span data-ttu-id="82d47-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82d47-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82d47-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82d47-137">JSON Representation</span></span>
<span data-ttu-id="82d47-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82d47-138">Here is a JSON representation of the resource.</span></span>
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



