---
title: tipo de recurso groupPolicyConfigurationAssignment
description: A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 367e6f2c38cb5ec07ce63de3724ec01d55ae68dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528109"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="cfd4a-103">tipo de recurso groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="cfd4a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cfd4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfd4a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfd4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfd4a-107">A entidade de atribuição configuração de política de grupo atribui um ou mais grupos AAD a uma configuração de política de grupo específica.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="cfd4a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cfd4a-108">Methods</span></span>
|<span data-ttu-id="cfd4a-109">Método</span><span class="sxs-lookup"><span data-stu-id="cfd4a-109">Method</span></span>|<span data-ttu-id="cfd4a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfd4a-110">Return Type</span></span>|<span data-ttu-id="cfd4a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfd4a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cfd4a-112">Listar groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="cfd4a-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="cfd4a-113">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cfd4a-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cfd4a-114">Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cfd4a-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="cfd4a-115">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="cfd4a-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="cfd4a-117">Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cfd4a-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="cfd4a-118">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="cfd4a-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="cfd4a-120">Criar um novo objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cfd4a-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="cfd4a-121">Excluir groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="cfd4a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfd4a-122">None</span></span>|<span data-ttu-id="cfd4a-123">Exclui [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cfd4a-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="cfd4a-124">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="cfd4a-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cfd4a-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="cfd4a-126">Atualiza as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cfd4a-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfd4a-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfd4a-127">Properties</span></span>
|<span data-ttu-id="cfd4a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfd4a-128">Property</span></span>|<span data-ttu-id="cfd4a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfd4a-129">Type</span></span>|<span data-ttu-id="cfd4a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfd4a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfd4a-131">id</span><span class="sxs-lookup"><span data-stu-id="cfd4a-131">id</span></span>|<span data-ttu-id="cfd4a-132">String</span><span class="sxs-lookup"><span data-stu-id="cfd4a-132">String</span></span>|<span data-ttu-id="cfd4a-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-133">Key of the entity.</span></span>|
|<span data-ttu-id="cfd4a-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfd4a-134">lastModifiedDateTime</span></span>|<span data-ttu-id="cfd4a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfd4a-135">DateTimeOffset</span></span>|<span data-ttu-id="cfd4a-136">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="cfd4a-137">destino</span><span class="sxs-lookup"><span data-stu-id="cfd4a-137">target</span></span>|[<span data-ttu-id="cfd4a-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cfd4a-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cfd4a-139">O tipo de grupo de destino da configuração da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfd4a-140">Relações</span><span class="sxs-lookup"><span data-stu-id="cfd4a-140">Relationships</span></span>
<span data-ttu-id="cfd4a-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfd4a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfd4a-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfd4a-142">JSON Representation</span></span>
<span data-ttu-id="cfd4a-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfd4a-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



