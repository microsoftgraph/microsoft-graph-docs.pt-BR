---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69c7fc6dc2a4a3ff90e14d430fba9b564930e0a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567897"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="96444-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="96444-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96444-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96444-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="96444-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="96444-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="96444-107">Methods</span></span>
|<span data-ttu-id="96444-108">Método</span><span class="sxs-lookup"><span data-stu-id="96444-108">Method</span></span>|<span data-ttu-id="96444-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96444-109">Return Type</span></span>|<span data-ttu-id="96444-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96444-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96444-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="96444-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="96444-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="96444-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="96444-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96444-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="96444-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="96444-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="96444-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96444-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="96444-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="96444-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="96444-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96444-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="96444-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="96444-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96444-121">None</span></span>|<span data-ttu-id="96444-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96444-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="96444-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="96444-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96444-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="96444-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96444-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96444-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96444-126">Properties</span></span>
|<span data-ttu-id="96444-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96444-127">Property</span></span>|<span data-ttu-id="96444-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="96444-128">Type</span></span>|<span data-ttu-id="96444-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="96444-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96444-130">id</span><span class="sxs-lookup"><span data-stu-id="96444-130">id</span></span>|<span data-ttu-id="96444-131">String</span><span class="sxs-lookup"><span data-stu-id="96444-131">String</span></span>|<span data-ttu-id="96444-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="96444-132">The key of the assignment.</span></span>|
|<span data-ttu-id="96444-133">destino</span><span class="sxs-lookup"><span data-stu-id="96444-133">target</span></span>|[<span data-ttu-id="96444-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="96444-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="96444-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96444-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96444-136">Relações</span><span class="sxs-lookup"><span data-stu-id="96444-136">Relationships</span></span>
<span data-ttu-id="96444-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96444-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96444-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96444-138">JSON Representation</span></span>
<span data-ttu-id="96444-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96444-139">Here is a JSON representation of the resource.</span></span>
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





