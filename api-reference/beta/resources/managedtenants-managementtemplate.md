---
title: Tipo de recurso managementTemplate
description: Representa um grupo de ações e configurações que podem ser executadas em um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2055db2d291dce3da0b4ad144c07b09bbb2fea6f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401996"
---
# <a name="managementtemplate-resource-type"></a><span data-ttu-id="217a6-103">Tipo de recurso managementTemplate</span><span class="sxs-lookup"><span data-stu-id="217a6-103">managementTemplate resource type</span></span>

<span data-ttu-id="217a6-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="217a6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="217a6-105">Representa um grupo de ações e configurações que podem ser executadas em um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="217a6-105">Represents a group of actions and setting that can be performed against a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="217a6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="217a6-106">Methods</span></span>
|<span data-ttu-id="217a6-107">Método</span><span class="sxs-lookup"><span data-stu-id="217a6-107">Method</span></span>|<span data-ttu-id="217a6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="217a6-108">Return type</span></span>|<span data-ttu-id="217a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="217a6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="217a6-110">Gerenciamento de listasTemplates</span><span class="sxs-lookup"><span data-stu-id="217a6-110">List managementTemplates</span></span>](../api/managedtenants-managedtenant-list-managementtemplates.md)|<span data-ttu-id="217a6-111">[coleção microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="217a6-111">[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection</span></span>|<span data-ttu-id="217a6-112">Obter uma lista dos [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="217a6-112">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>|
|[<span data-ttu-id="217a6-113">Obter managementTemplate</span><span class="sxs-lookup"><span data-stu-id="217a6-113">Get managementTemplate</span></span>](../api/managedtenants-managementtemplate-get.md)|[<span data-ttu-id="217a6-114">microsoft.graph.managedTenants.managementTemplate</span><span class="sxs-lookup"><span data-stu-id="217a6-114">microsoft.graph.managedTenants.managementTemplate</span></span>](../resources/managedtenants-managementtemplate.md)|<span data-ttu-id="217a6-115">Leia as propriedades e as relações de um [objeto managementTemplate.](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="217a6-115">Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="217a6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="217a6-116">Properties</span></span>
|<span data-ttu-id="217a6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="217a6-117">Property</span></span>|<span data-ttu-id="217a6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="217a6-118">Type</span></span>|<span data-ttu-id="217a6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="217a6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="217a6-120">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="217a6-120">category</span></span>|<span data-ttu-id="217a6-121">managementCategory</span><span class="sxs-lookup"><span data-stu-id="217a6-121">managementCategory</span></span>|<span data-ttu-id="217a6-122">A categoria de gerenciamento do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-122">The management category for the management template.</span></span> <span data-ttu-id="217a6-123">Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="217a6-123">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="217a6-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="217a6-124">Required.</span></span> <span data-ttu-id="217a6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-125">Read-only.</span></span>|
|<span data-ttu-id="217a6-126">description</span><span class="sxs-lookup"><span data-stu-id="217a6-126">description</span></span>|<span data-ttu-id="217a6-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="217a6-127">String</span></span>|<span data-ttu-id="217a6-128">A descrição do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-128">The description for the management template.</span></span> <span data-ttu-id="217a6-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="217a6-129">Optional.</span></span> <span data-ttu-id="217a6-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-130">Read-only.</span></span>|
|<span data-ttu-id="217a6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="217a6-131">displayName</span></span>|<span data-ttu-id="217a6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="217a6-132">String</span></span>|<span data-ttu-id="217a6-133">O nome de exibição do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-133">The display name for the management template.</span></span> <span data-ttu-id="217a6-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="217a6-134">Required.</span></span> <span data-ttu-id="217a6-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-135">Read-only.</span></span>|
|<span data-ttu-id="217a6-136">id</span><span class="sxs-lookup"><span data-stu-id="217a6-136">id</span></span>|<span data-ttu-id="217a6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="217a6-137">String</span></span>|<span data-ttu-id="217a6-138">O identificador exclusivo do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-138">The unique identifier for the management template.</span></span> <span data-ttu-id="217a6-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="217a6-139">Required.</span></span> <span data-ttu-id="217a6-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-140">Read-only.</span></span>|
|<span data-ttu-id="217a6-141">parameters</span><span class="sxs-lookup"><span data-stu-id="217a6-141">parameters</span></span>|<span data-ttu-id="217a6-142">[coleção microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md)</span><span class="sxs-lookup"><span data-stu-id="217a6-142">[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) collection</span></span>|<span data-ttu-id="217a6-143">A coleção de parâmetros usados pelo modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-143">The collection of parameters used by the management template.</span></span> <span data-ttu-id="217a6-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="217a6-144">Optional.</span></span> <span data-ttu-id="217a6-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-145">Read-only.</span></span>|
|<span data-ttu-id="217a6-146">workloadActions</span><span class="sxs-lookup"><span data-stu-id="217a6-146">workloadActions</span></span>|<span data-ttu-id="217a6-147">[coleção microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)</span><span class="sxs-lookup"><span data-stu-id="217a6-147">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="217a6-148">O conjunto de ações de carga de trabalho associadas ao modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="217a6-148">The collection of workload actions associated with the management template.</span></span> <span data-ttu-id="217a6-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="217a6-149">Optional.</span></span> <span data-ttu-id="217a6-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="217a6-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="217a6-151">Relações</span><span class="sxs-lookup"><span data-stu-id="217a6-151">Relationships</span></span>
<span data-ttu-id="217a6-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="217a6-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="217a6-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="217a6-153">JSON representation</span></span>
<span data-ttu-id="217a6-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="217a6-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
