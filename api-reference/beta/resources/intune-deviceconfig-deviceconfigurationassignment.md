---
title: Tipo de recurso deviceConfigurationAssignment
description: A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 115cbd779e53f303bdbf95dc28916879726676ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402598"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="6271c-103">Tipo de recurso deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="6271c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6271c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6271c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6271c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6271c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6271c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6271c-107">A entidade de atribuição de configuração do dispositivo atribui um grupo AAD a uma configuração de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="6271c-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="6271c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6271c-108">Methods</span></span>
|<span data-ttu-id="6271c-109">Método</span><span class="sxs-lookup"><span data-stu-id="6271c-109">Method</span></span>|<span data-ttu-id="6271c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6271c-110">Return Type</span></span>|<span data-ttu-id="6271c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6271c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6271c-112">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="6271c-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="6271c-113">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6271c-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6271c-114">Listar propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6271c-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="6271c-115">Obter deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="6271c-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6271c-117">Ler propriedades e relações de objetos de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6271c-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6271c-118">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="6271c-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6271c-120">Criar um novo objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6271c-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6271c-121">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="6271c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6271c-122">None</span></span>|<span data-ttu-id="6271c-123">Excluir [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6271c-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="6271c-124">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="6271c-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6271c-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="6271c-126">Atualizar as propriedades de um objeto de [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6271c-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6271c-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6271c-127">Properties</span></span>
|<span data-ttu-id="6271c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6271c-128">Property</span></span>|<span data-ttu-id="6271c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6271c-129">Type</span></span>|<span data-ttu-id="6271c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6271c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6271c-131">id</span><span class="sxs-lookup"><span data-stu-id="6271c-131">id</span></span>|<span data-ttu-id="6271c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6271c-132">String</span></span>|<span data-ttu-id="6271c-133">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6271c-133">The key of the assignment.</span></span>|
|<span data-ttu-id="6271c-134">destino</span><span class="sxs-lookup"><span data-stu-id="6271c-134">target</span></span>|[<span data-ttu-id="6271c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6271c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6271c-136">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6271c-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6271c-137">Relações</span><span class="sxs-lookup"><span data-stu-id="6271c-137">Relationships</span></span>
<span data-ttu-id="6271c-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6271c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6271c-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6271c-139">JSON Representation</span></span>
<span data-ttu-id="6271c-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6271c-140">Here is a JSON representation of the resource.</span></span>
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




