---
title: Tipo de recurso managedDeviceMobileAppConfigurationAssignment
description: Contém as propriedades usadas para atribuir uma configuração de aplicativo MDM a um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c04947c63a72ebb1476ce5c863731a876987d603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830174"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="b72c8-103">Tipo de recurso managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="b72c8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b72c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b72c8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b72c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b72c8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b72c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b72c8-107">Contém as propriedades usadas para atribuir uma configuração de aplicativo MDM a um grupo.</span><span class="sxs-lookup"><span data-stu-id="b72c8-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="b72c8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b72c8-108">Methods</span></span>
|<span data-ttu-id="b72c8-109">Método</span><span class="sxs-lookup"><span data-stu-id="b72c8-109">Method</span></span>|<span data-ttu-id="b72c8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b72c8-110">Return Type</span></span>|<span data-ttu-id="b72c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b72c8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b72c8-112">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="b72c8-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="b72c8-113">Conjunto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b72c8-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b72c8-114">Listar propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b72c8-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="b72c8-115">Obter managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="b72c8-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="b72c8-117">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b72c8-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b72c8-118">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="b72c8-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="b72c8-120">Criar um novo objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b72c8-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b72c8-121">Excluir managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="b72c8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b72c8-122">None</span></span>|<span data-ttu-id="b72c8-123">Excluir um [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b72c8-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="b72c8-124">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="b72c8-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b72c8-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="b72c8-126">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b72c8-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b72c8-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b72c8-127">Properties</span></span>
|<span data-ttu-id="b72c8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b72c8-128">Property</span></span>|<span data-ttu-id="b72c8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b72c8-129">Type</span></span>|<span data-ttu-id="b72c8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b72c8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b72c8-131">id</span><span class="sxs-lookup"><span data-stu-id="b72c8-131">id</span></span>|<span data-ttu-id="b72c8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b72c8-132">String</span></span>|<span data-ttu-id="b72c8-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="b72c8-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b72c8-134">destino</span><span class="sxs-lookup"><span data-stu-id="b72c8-134">target</span></span>|[<span data-ttu-id="b72c8-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b72c8-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b72c8-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="b72c8-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b72c8-137">Relações</span><span class="sxs-lookup"><span data-stu-id="b72c8-137">Relationships</span></span>
<span data-ttu-id="b72c8-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b72c8-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b72c8-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b72c8-139">JSON Representation</span></span>
<span data-ttu-id="b72c8-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b72c8-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





