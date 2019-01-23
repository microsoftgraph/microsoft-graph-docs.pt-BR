---
title: tipo de recurso de groupPolicyConfigurationAssignment
description: A entidade de atribuição de configuração de diretiva de grupo atribui um ou mais grupos AAD para uma configuração de diretiva de grupo específico.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 508581ba7b5ac689338c179f4f6b211928c9abaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429037"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="4af3b-103">tipo de recurso de groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="4af3b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4af3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4af3b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4af3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4af3b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4af3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4af3b-107">A entidade de atribuição de configuração de diretiva de grupo atribui um ou mais grupos AAD para uma configuração de diretiva de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="4af3b-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="4af3b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4af3b-108">Methods</span></span>
|<span data-ttu-id="4af3b-109">Método</span><span class="sxs-lookup"><span data-stu-id="4af3b-109">Method</span></span>|<span data-ttu-id="4af3b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4af3b-110">Return Type</span></span>|<span data-ttu-id="4af3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af3b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4af3b-112">Lista groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="4af3b-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="4af3b-113">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4af3b-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4af3b-114">Lista as propriedades e os relacionamentos dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4af3b-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="4af3b-115">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="4af3b-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4af3b-117">Leia as propriedades e os relacionamentos do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4af3b-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4af3b-118">Criar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="4af3b-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4af3b-120">Crie um novo objeto de [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4af3b-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4af3b-121">Excluir groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="4af3b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4af3b-122">None</span></span>|<span data-ttu-id="4af3b-123">Exclui um [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4af3b-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="4af3b-124">Atualizar groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="4af3b-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4af3b-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4af3b-126">Atualize as propriedades de um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4af3b-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4af3b-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4af3b-127">Properties</span></span>
|<span data-ttu-id="4af3b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4af3b-128">Property</span></span>|<span data-ttu-id="4af3b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4af3b-129">Type</span></span>|<span data-ttu-id="4af3b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af3b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4af3b-131">id</span><span class="sxs-lookup"><span data-stu-id="4af3b-131">id</span></span>|<span data-ttu-id="4af3b-132">String</span><span class="sxs-lookup"><span data-stu-id="4af3b-132">String</span></span>|<span data-ttu-id="4af3b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4af3b-133">Key of the entity.</span></span>|
|<span data-ttu-id="4af3b-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4af3b-134">lastModifiedDateTime</span></span>|<span data-ttu-id="4af3b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4af3b-135">DateTimeOffset</span></span>|<span data-ttu-id="4af3b-136">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4af3b-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="4af3b-137">destino</span><span class="sxs-lookup"><span data-stu-id="4af3b-137">target</span></span>|[<span data-ttu-id="4af3b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4af3b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4af3b-139">O tipo de grupos direcionadas a configuração de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="4af3b-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4af3b-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4af3b-140">Relationships</span></span>
<span data-ttu-id="4af3b-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4af3b-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4af3b-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4af3b-142">JSON Representation</span></span>
<span data-ttu-id="4af3b-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4af3b-143">Here is a JSON representation of the resource.</span></span>
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




