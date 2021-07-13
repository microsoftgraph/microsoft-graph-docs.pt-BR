---
title: Tipo de recurso managementAction
description: Representa uma ação de gerenciamento de linha de base para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402144"
---
# <a name="managementaction-resource-type"></a><span data-ttu-id="60039-103">Tipo de recurso managementAction</span><span class="sxs-lookup"><span data-stu-id="60039-103">managementAction resource type</span></span>

<span data-ttu-id="60039-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="60039-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60039-105">Representa uma ação de gerenciamento de linha de base para um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="60039-105">Represents a baseline management action for a given managed tenant.</span></span> <span data-ttu-id="60039-106">Exemplos de ações de gerenciamento são criptografia de dispositivo, configurações para permitir Azure Active Directory registro de dispositivos e exigir autenticação multifa factor para administradores.</span><span class="sxs-lookup"><span data-stu-id="60039-106">Examples of management actions are device encryption, perform configurations to allow Azure Active Directory device enrollment, and require multi-factor authentication for admins.</span></span>

## <a name="methods"></a><span data-ttu-id="60039-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="60039-107">Methods</span></span>
|<span data-ttu-id="60039-108">Método</span><span class="sxs-lookup"><span data-stu-id="60039-108">Method</span></span>|<span data-ttu-id="60039-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60039-109">Return type</span></span>|<span data-ttu-id="60039-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="60039-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60039-111">Gerenciamento de listasActions</span><span class="sxs-lookup"><span data-stu-id="60039-111">List managementActions</span></span>](../api/managedtenants-managedtenant-list-managementactions.md)|<span data-ttu-id="60039-112">[Coleção microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="60039-112">[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) collection</span></span>|<span data-ttu-id="60039-113">Obter uma lista dos [objetos managementAction](../resources/managedtenants-managementaction.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="60039-113">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>|
|[<span data-ttu-id="60039-114">Obter managementAction</span><span class="sxs-lookup"><span data-stu-id="60039-114">Get managementAction</span></span>](../api/managedtenants-managementaction-get.md)|[<span data-ttu-id="60039-115">microsoft.graph.managedTenants.managementAction</span><span class="sxs-lookup"><span data-stu-id="60039-115">microsoft.graph.managedTenants.managementAction</span></span>](../resources/managedtenants-managementaction.md)|<span data-ttu-id="60039-116">Leia as propriedades e as relações de um [objeto managementAction.](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="60039-116">Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.</span></span>|
|[<span data-ttu-id="60039-117">apply</span><span class="sxs-lookup"><span data-stu-id="60039-117">apply</span></span>](../api/managedtenants-managementaction-apply.md)|[<span data-ttu-id="60039-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="60039-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span></span>](../resources/managedtenants-managementactiondeploymentstatus.md)|<span data-ttu-id="60039-119">Aplica as ações de gerenciamento ao locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="60039-119">Applies the management actions against the managed tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="60039-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60039-120">Properties</span></span>
|<span data-ttu-id="60039-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60039-121">Property</span></span>|<span data-ttu-id="60039-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="60039-122">Type</span></span>|<span data-ttu-id="60039-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="60039-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60039-124">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="60039-124">category</span></span>|<span data-ttu-id="60039-125">managementCategory</span><span class="sxs-lookup"><span data-stu-id="60039-125">managementCategory</span></span>|<span data-ttu-id="60039-126">A categoria da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-126">The category for the management action.</span></span> <span data-ttu-id="60039-127">Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="60039-127">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="60039-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="60039-128">Optional.</span></span> <span data-ttu-id="60039-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-129">Read-only.</span></span>|
|<span data-ttu-id="60039-130">description</span><span class="sxs-lookup"><span data-stu-id="60039-130">description</span></span>|<span data-ttu-id="60039-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60039-131">String</span></span>|<span data-ttu-id="60039-132">A descrição da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-132">The description for the management action.</span></span> <span data-ttu-id="60039-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="60039-133">Optional.</span></span> <span data-ttu-id="60039-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-134">Read-only.</span></span>|
|<span data-ttu-id="60039-135">displayName</span><span class="sxs-lookup"><span data-stu-id="60039-135">displayName</span></span>|<span data-ttu-id="60039-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60039-136">String</span></span>|<span data-ttu-id="60039-137">O nome de exibição da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-137">The display name for the management action.</span></span> <span data-ttu-id="60039-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="60039-138">Optional.</span></span> <span data-ttu-id="60039-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-139">Read-only.</span></span>|
|<span data-ttu-id="60039-140">id</span><span class="sxs-lookup"><span data-stu-id="60039-140">id</span></span>|<span data-ttu-id="60039-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60039-141">String</span></span>|<span data-ttu-id="60039-142">O identificador exclusivo da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-142">The unique identifier for the management action.</span></span> <span data-ttu-id="60039-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60039-143">Required.</span></span> <span data-ttu-id="60039-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-144">Read-only.</span></span>|
|<span data-ttu-id="60039-145">referenceTemplateId</span><span class="sxs-lookup"><span data-stu-id="60039-145">referenceTemplateId</span></span>|<span data-ttu-id="60039-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60039-146">String</span></span>|<span data-ttu-id="60039-147">A referência para o modelo de gerenciamento usado para gerar a ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-147">The reference for the management template used to generate the management action.</span></span> <span data-ttu-id="60039-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60039-148">Required.</span></span> <span data-ttu-id="60039-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-149">Read-only.</span></span>|
|<span data-ttu-id="60039-150">workloadActions</span><span class="sxs-lookup"><span data-stu-id="60039-150">workloadActions</span></span>|<span data-ttu-id="60039-151">[coleção microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)</span><span class="sxs-lookup"><span data-stu-id="60039-151">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="60039-152">O conjunto de ações de carga de trabalho associadas à ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="60039-152">The collection of workload actions associated with the management action.</span></span> <span data-ttu-id="60039-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60039-153">Required.</span></span> <span data-ttu-id="60039-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60039-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60039-155">Relações</span><span class="sxs-lookup"><span data-stu-id="60039-155">Relationships</span></span>
<span data-ttu-id="60039-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60039-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60039-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60039-157">JSON representation</span></span>
<span data-ttu-id="60039-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60039-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
