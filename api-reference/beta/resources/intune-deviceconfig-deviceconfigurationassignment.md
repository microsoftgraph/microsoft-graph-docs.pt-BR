---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69c7fc6dc2a4a3ff90e14d430fba9b564930e0a7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774719"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="09e0c-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="09e0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09e0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09e0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09e0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09e0c-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="09e0c-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="09e0c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="09e0c-107">Methods</span></span>
|<span data-ttu-id="09e0c-108">Método</span><span class="sxs-lookup"><span data-stu-id="09e0c-108">Method</span></span>|<span data-ttu-id="09e0c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09e0c-109">Return Type</span></span>|<span data-ttu-id="09e0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09e0c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09e0c-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="09e0c-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="09e0c-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09e0c-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="09e0c-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e0c-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="09e0c-114">Acessar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="09e0c-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="09e0c-116">Leia as propriedades e as relações do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e0c-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="09e0c-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="09e0c-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="09e0c-119">Criar um novo objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e0c-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="09e0c-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="09e0c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09e0c-121">None</span></span>|<span data-ttu-id="09e0c-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e0c-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="09e0c-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="09e0c-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0c-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="09e0c-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e0c-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09e0c-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09e0c-126">Properties</span></span>
|<span data-ttu-id="09e0c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09e0c-127">Property</span></span>|<span data-ttu-id="09e0c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="09e0c-128">Type</span></span>|<span data-ttu-id="09e0c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="09e0c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e0c-130">id</span><span class="sxs-lookup"><span data-stu-id="09e0c-130">id</span></span>|<span data-ttu-id="09e0c-131">String</span><span class="sxs-lookup"><span data-stu-id="09e0c-131">String</span></span>|<span data-ttu-id="09e0c-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="09e0c-132">The key of the assignment.</span></span>|
|<span data-ttu-id="09e0c-133">destino</span><span class="sxs-lookup"><span data-stu-id="09e0c-133">target</span></span>|[<span data-ttu-id="09e0c-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="09e0c-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="09e0c-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09e0c-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09e0c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="09e0c-136">Relationships</span></span>
<span data-ttu-id="09e0c-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="09e0c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09e0c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09e0c-138">JSON Representation</span></span>
<span data-ttu-id="09e0c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09e0c-139">Here is a JSON representation of the resource.</span></span>
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





