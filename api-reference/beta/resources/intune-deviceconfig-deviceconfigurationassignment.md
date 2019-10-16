---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af6c3715e106e446d76c1e7b250e79e713cef079
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538886"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="a082f-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="a082f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a082f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a082f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a082f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a082f-106">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="a082f-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="a082f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a082f-107">Methods</span></span>
|<span data-ttu-id="a082f-108">Método</span><span class="sxs-lookup"><span data-stu-id="a082f-108">Method</span></span>|<span data-ttu-id="a082f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a082f-109">Return Type</span></span>|<span data-ttu-id="a082f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a082f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a082f-111">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a082f-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="a082f-112">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a082f-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a082f-113">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a082f-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="a082f-114">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="a082f-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a082f-116">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a082f-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a082f-117">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="a082f-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a082f-119">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a082f-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a082f-120">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="a082f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a082f-121">None</span></span>|<span data-ttu-id="a082f-122">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a082f-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="a082f-123">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="a082f-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a082f-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a082f-125">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a082f-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a082f-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a082f-126">Properties</span></span>
|<span data-ttu-id="a082f-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a082f-127">Property</span></span>|<span data-ttu-id="a082f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a082f-128">Type</span></span>|<span data-ttu-id="a082f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a082f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a082f-130">id</span><span class="sxs-lookup"><span data-stu-id="a082f-130">id</span></span>|<span data-ttu-id="a082f-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a082f-131">String</span></span>|<span data-ttu-id="a082f-132">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a082f-132">The key of the assignment.</span></span>|
|<span data-ttu-id="a082f-133">destino</span><span class="sxs-lookup"><span data-stu-id="a082f-133">target</span></span>|[<span data-ttu-id="a082f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a082f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a082f-135">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a082f-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="a082f-136">source</span><span class="sxs-lookup"><span data-stu-id="a082f-136">source</span></span>|[<span data-ttu-id="a082f-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a082f-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a082f-138">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="a082f-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="a082f-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a082f-139">This property is read-only.</span></span> <span data-ttu-id="a082f-140">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a082f-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a082f-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="a082f-141">sourceId</span></span>|<span data-ttu-id="a082f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a082f-142">String</span></span>|<span data-ttu-id="a082f-143">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a082f-143">The identifier of the source of the assignment.</span></span> <span data-ttu-id="a082f-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a082f-144">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a082f-145">Relações</span><span class="sxs-lookup"><span data-stu-id="a082f-145">Relationships</span></span>
<span data-ttu-id="a082f-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a082f-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a082f-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a082f-147">JSON Representation</span></span>
<span data-ttu-id="a082f-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a082f-148">Here is a JSON representation of the resource.</span></span>
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
  },
  "source": "String",
  "sourceId": "String"
}
```



