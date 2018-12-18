---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
ms.openlocfilehash: 26afc67312ab8544b395b5e20b89a01558fc75d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306241"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="6a653-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="6a653-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a653-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a653-105">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="6a653-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="6a653-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a653-106">Methods</span></span>
|<span data-ttu-id="6a653-107">Método</span><span class="sxs-lookup"><span data-stu-id="6a653-107">Method</span></span>|<span data-ttu-id="6a653-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a653-108">Return Type</span></span>|<span data-ttu-id="6a653-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a653-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a653-110">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="6a653-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="6a653-111">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6a653-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6a653-112">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a653-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="6a653-113">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="6a653-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6a653-115">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a653-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6a653-116">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="6a653-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6a653-118">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a653-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6a653-119">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="6a653-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a653-120">None</span></span>|<span data-ttu-id="6a653-121">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a653-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="6a653-122">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="6a653-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a653-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6a653-124">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a653-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a653-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a653-125">Properties</span></span>
|<span data-ttu-id="6a653-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a653-126">Property</span></span>|<span data-ttu-id="6a653-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a653-127">Type</span></span>|<span data-ttu-id="6a653-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a653-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a653-129">id</span><span class="sxs-lookup"><span data-stu-id="6a653-129">id</span></span>|<span data-ttu-id="6a653-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a653-130">String</span></span>|<span data-ttu-id="6a653-131">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6a653-131">The key of the assignment.</span></span>|
|<span data-ttu-id="6a653-132">destino</span><span class="sxs-lookup"><span data-stu-id="6a653-132">target</span></span>|[<span data-ttu-id="6a653-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6a653-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6a653-134">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a653-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a653-135">Relações</span><span class="sxs-lookup"><span data-stu-id="6a653-135">Relationships</span></span>
<span data-ttu-id="6a653-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a653-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a653-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a653-137">JSON Representation</span></span>
<span data-ttu-id="6a653-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a653-138">Here is a JSON representation of the resource.</span></span>
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



