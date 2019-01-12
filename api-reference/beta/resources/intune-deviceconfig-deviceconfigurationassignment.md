---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7860a7526fc3b0251f4d9b07974170039d4c3312
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991969"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="84ebe-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="84ebe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84ebe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84ebe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84ebe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84ebe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84ebe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84ebe-107">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="84ebe-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="84ebe-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="84ebe-108">Methods</span></span>
|<span data-ttu-id="84ebe-109">Método</span><span class="sxs-lookup"><span data-stu-id="84ebe-109">Method</span></span>|<span data-ttu-id="84ebe-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="84ebe-110">Return Type</span></span>|<span data-ttu-id="84ebe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ebe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84ebe-112">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="84ebe-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="84ebe-113">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="84ebe-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="84ebe-114">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84ebe-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="84ebe-115">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="84ebe-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="84ebe-117">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84ebe-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="84ebe-118">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="84ebe-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="84ebe-120">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84ebe-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="84ebe-121">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="84ebe-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84ebe-122">None</span></span>|<span data-ttu-id="84ebe-123">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84ebe-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="84ebe-124">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="84ebe-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="84ebe-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="84ebe-126">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84ebe-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84ebe-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84ebe-127">Properties</span></span>
|<span data-ttu-id="84ebe-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84ebe-128">Property</span></span>|<span data-ttu-id="84ebe-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="84ebe-129">Type</span></span>|<span data-ttu-id="84ebe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ebe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ebe-131">id</span><span class="sxs-lookup"><span data-stu-id="84ebe-131">id</span></span>|<span data-ttu-id="84ebe-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84ebe-132">String</span></span>|<span data-ttu-id="84ebe-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="84ebe-133">The key of the assignment.</span></span>|
|<span data-ttu-id="84ebe-134">destino</span><span class="sxs-lookup"><span data-stu-id="84ebe-134">target</span></span>|[<span data-ttu-id="84ebe-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="84ebe-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="84ebe-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84ebe-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84ebe-137">Relações</span><span class="sxs-lookup"><span data-stu-id="84ebe-137">Relationships</span></span>
<span data-ttu-id="84ebe-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84ebe-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84ebe-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84ebe-139">JSON Representation</span></span>
<span data-ttu-id="84ebe-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84ebe-140">Here is a JSON representation of the resource.</span></span>
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





