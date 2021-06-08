---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f5c1e81b451a08cbfc5cf4d793d920dd01aebcde
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760096"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="94b8a-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="94b8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94b8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94b8a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94b8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94b8a-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="94b8a-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="94b8a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="94b8a-107">Methods</span></span>
|<span data-ttu-id="94b8a-108">Método</span><span class="sxs-lookup"><span data-stu-id="94b8a-108">Method</span></span>|<span data-ttu-id="94b8a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="94b8a-109">Return Type</span></span>|<span data-ttu-id="94b8a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94b8a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94b8a-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="94b8a-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="94b8a-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="94b8a-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="94b8a-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94b8a-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="94b8a-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="94b8a-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="94b8a-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94b8a-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="94b8a-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="94b8a-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="94b8a-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94b8a-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="94b8a-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="94b8a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94b8a-121">None</span></span>|<span data-ttu-id="94b8a-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94b8a-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="94b8a-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="94b8a-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="94b8a-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="94b8a-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94b8a-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94b8a-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94b8a-126">Properties</span></span>
|<span data-ttu-id="94b8a-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94b8a-127">Property</span></span>|<span data-ttu-id="94b8a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="94b8a-128">Type</span></span>|<span data-ttu-id="94b8a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="94b8a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b8a-130">id</span><span class="sxs-lookup"><span data-stu-id="94b8a-130">id</span></span>|<span data-ttu-id="94b8a-131">String</span><span class="sxs-lookup"><span data-stu-id="94b8a-131">String</span></span>|<span data-ttu-id="94b8a-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="94b8a-132">The key of the assignment.</span></span>|
|<span data-ttu-id="94b8a-133">destino</span><span class="sxs-lookup"><span data-stu-id="94b8a-133">target</span></span>|[<span data-ttu-id="94b8a-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="94b8a-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="94b8a-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94b8a-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94b8a-136">Relações</span><span class="sxs-lookup"><span data-stu-id="94b8a-136">Relationships</span></span>
<span data-ttu-id="94b8a-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94b8a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94b8a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94b8a-138">JSON Representation</span></span>
<span data-ttu-id="94b8a-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94b8a-139">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




