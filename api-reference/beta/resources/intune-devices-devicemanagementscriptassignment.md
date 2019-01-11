---
title: tipo de recurso de deviceManagementScriptAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc2da31d105ce9a8169607f3910c41801d86eb2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858748"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="6bd9d-103">tipo de recurso de deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="6bd9d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bd9d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bd9d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bd9d-107">Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="6bd9d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6bd9d-108">Methods</span></span>
|<span data-ttu-id="6bd9d-109">Método</span><span class="sxs-lookup"><span data-stu-id="6bd9d-109">Method</span></span>|<span data-ttu-id="6bd9d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6bd9d-110">Return Type</span></span>|<span data-ttu-id="6bd9d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd9d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bd9d-112">Lista deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="6bd9d-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="6bd9d-113">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6bd9d-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="6bd9d-114">Lista as propriedades e os relacionamentos dos objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd9d-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="6bd9d-115">Obter deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="6bd9d-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="6bd9d-117">Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd9d-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="6bd9d-118">Criar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="6bd9d-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="6bd9d-120">Crie um novo objeto de [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd9d-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="6bd9d-121">Excluir deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="6bd9d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bd9d-122">None</span></span>|<span data-ttu-id="6bd9d-123">Exclui um [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6bd9d-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="6bd9d-124">Atualizar deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="6bd9d-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6bd9d-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="6bd9d-126">Atualize as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd9d-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bd9d-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bd9d-127">Properties</span></span>
|<span data-ttu-id="6bd9d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bd9d-128">Property</span></span>|<span data-ttu-id="6bd9d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bd9d-129">Type</span></span>|<span data-ttu-id="6bd9d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd9d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bd9d-131">id</span><span class="sxs-lookup"><span data-stu-id="6bd9d-131">id</span></span>|<span data-ttu-id="6bd9d-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd9d-132">String</span></span>|<span data-ttu-id="6bd9d-133">Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="6bd9d-134">destino</span><span class="sxs-lookup"><span data-stu-id="6bd9d-134">target</span></span>|[<span data-ttu-id="6bd9d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6bd9d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6bd9d-136">A Id de grupo do Active Directory do Windows Azure Pretendemos o script.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bd9d-137">Relações</span><span class="sxs-lookup"><span data-stu-id="6bd9d-137">Relationships</span></span>
<span data-ttu-id="6bd9d-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bd9d-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bd9d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bd9d-139">JSON Representation</span></span>
<span data-ttu-id="6bd9d-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bd9d-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





