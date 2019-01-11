---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8031566663d9113fa40014bdb7bdd7603d3c6174
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842417"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="31a14-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="31a14-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31a14-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31a14-105">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="31a14-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="31a14-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="31a14-106">Methods</span></span>
|<span data-ttu-id="31a14-107">Método</span><span class="sxs-lookup"><span data-stu-id="31a14-107">Method</span></span>|<span data-ttu-id="31a14-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="31a14-108">Return Type</span></span>|<span data-ttu-id="31a14-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="31a14-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31a14-110">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="31a14-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="31a14-111">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="31a14-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="31a14-112">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a14-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="31a14-113">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="31a14-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="31a14-115">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a14-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="31a14-116">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="31a14-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="31a14-118">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a14-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="31a14-119">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="31a14-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31a14-120">None</span></span>|<span data-ttu-id="31a14-121">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a14-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="31a14-122">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="31a14-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31a14-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="31a14-124">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a14-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31a14-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31a14-125">Properties</span></span>
|<span data-ttu-id="31a14-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31a14-126">Property</span></span>|<span data-ttu-id="31a14-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="31a14-127">Type</span></span>|<span data-ttu-id="31a14-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="31a14-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a14-129">id</span><span class="sxs-lookup"><span data-stu-id="31a14-129">id</span></span>|<span data-ttu-id="31a14-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31a14-130">String</span></span>|<span data-ttu-id="31a14-131">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="31a14-131">The key of the assignment.</span></span>|
|<span data-ttu-id="31a14-132">destino</span><span class="sxs-lookup"><span data-stu-id="31a14-132">target</span></span>|[<span data-ttu-id="31a14-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="31a14-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="31a14-134">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31a14-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a14-135">Relações</span><span class="sxs-lookup"><span data-stu-id="31a14-135">Relationships</span></span>
<span data-ttu-id="31a14-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31a14-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31a14-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31a14-137">JSON Representation</span></span>
<span data-ttu-id="31a14-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31a14-138">Here is a JSON representation of the resource.</span></span>
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



