---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 086ff1f3c9d06a1afe394afff0bd7ee6c543804d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888694"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="359db-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="359db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="359db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="359db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="359db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="359db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="359db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="359db-107">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="359db-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="359db-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="359db-108">Methods</span></span>
|<span data-ttu-id="359db-109">Método</span><span class="sxs-lookup"><span data-stu-id="359db-109">Method</span></span>|<span data-ttu-id="359db-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="359db-110">Return Type</span></span>|<span data-ttu-id="359db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="359db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="359db-112">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="359db-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="359db-113">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="359db-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="359db-114">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="359db-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="359db-115">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="359db-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="359db-117">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="359db-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="359db-118">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="359db-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="359db-120">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="359db-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="359db-121">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="359db-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="359db-122">None</span></span>|<span data-ttu-id="359db-123">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="359db-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="359db-124">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="359db-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="359db-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="359db-126">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="359db-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="359db-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="359db-127">Properties</span></span>
|<span data-ttu-id="359db-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="359db-128">Property</span></span>|<span data-ttu-id="359db-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="359db-129">Type</span></span>|<span data-ttu-id="359db-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="359db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="359db-131">id</span><span class="sxs-lookup"><span data-stu-id="359db-131">id</span></span>|<span data-ttu-id="359db-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="359db-132">String</span></span>|<span data-ttu-id="359db-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="359db-133">The key of the assignment.</span></span>|
|<span data-ttu-id="359db-134">destino</span><span class="sxs-lookup"><span data-stu-id="359db-134">target</span></span>|[<span data-ttu-id="359db-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="359db-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="359db-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="359db-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="359db-137">Relações</span><span class="sxs-lookup"><span data-stu-id="359db-137">Relationships</span></span>
<span data-ttu-id="359db-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="359db-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="359db-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="359db-139">JSON Representation</span></span>
<span data-ttu-id="359db-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="359db-140">Here is a JSON representation of the resource.</span></span>
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





