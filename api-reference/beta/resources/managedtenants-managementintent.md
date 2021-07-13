---
title: tipo de recurso managementIntent
description: Representa metadados para uma linha de base e quais modelos de gerenciamento estão incluídos.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7648da23e5d49a9bd2910c2ccbde7e676a1d7cd0
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401998"
---
# <a name="managementintent-resource-type"></a><span data-ttu-id="aa511-103">tipo de recurso managementIntent</span><span class="sxs-lookup"><span data-stu-id="aa511-103">managementIntent resource type</span></span>

<span data-ttu-id="aa511-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="aa511-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa511-105">Representa metadados para uma linha de base e quais modelos de gerenciamento estão incluídos.</span><span class="sxs-lookup"><span data-stu-id="aa511-105">Represents metadata for a baseline and what management templates are included.</span></span>

## <a name="methods"></a><span data-ttu-id="aa511-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="aa511-106">Methods</span></span>
|<span data-ttu-id="aa511-107">Método</span><span class="sxs-lookup"><span data-stu-id="aa511-107">Method</span></span>|<span data-ttu-id="aa511-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aa511-108">Return type</span></span>|<span data-ttu-id="aa511-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa511-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa511-110">Gerenciamento de listaIntents</span><span class="sxs-lookup"><span data-stu-id="aa511-110">List managementIntents</span></span>](../api/managedtenants-managedtenant-list-managementintents.md)|<span data-ttu-id="aa511-111">[coleção microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="aa511-111">[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) collection</span></span>|<span data-ttu-id="aa511-112">Obter uma lista dos [objetos managementIntent](../resources/managedtenants-managementintent.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="aa511-112">Get a list of the [managementIntent](../resources/managedtenants-managementintent.md) objects and their properties.</span></span>|
|[<span data-ttu-id="aa511-113">Obter managementIntent</span><span class="sxs-lookup"><span data-stu-id="aa511-113">Get managementIntent</span></span>](../api/managedtenants-managementintent-get.md)|[<span data-ttu-id="aa511-114">microsoft.graph.managedTenants.managementIntent</span><span class="sxs-lookup"><span data-stu-id="aa511-114">microsoft.graph.managedTenants.managementIntent</span></span>](../resources/managedtenants-managementintent.md)|<span data-ttu-id="aa511-115">Leia as propriedades e as relações de um [objeto managementIntent.](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="aa511-115">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa511-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa511-116">Properties</span></span>
|<span data-ttu-id="aa511-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa511-117">Property</span></span>|<span data-ttu-id="aa511-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa511-118">Type</span></span>|<span data-ttu-id="aa511-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa511-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa511-120">displayName</span><span class="sxs-lookup"><span data-stu-id="aa511-120">displayName</span></span>|<span data-ttu-id="aa511-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa511-121">String</span></span>|<span data-ttu-id="aa511-122">O nome de exibição para a intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="aa511-122">The display name for the management intent.</span></span> <span data-ttu-id="aa511-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa511-123">Optional.</span></span> <span data-ttu-id="aa511-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa511-124">Read-only.</span></span>|
|<span data-ttu-id="aa511-125">id</span><span class="sxs-lookup"><span data-stu-id="aa511-125">id</span></span>|<span data-ttu-id="aa511-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa511-126">String</span></span>|<span data-ttu-id="aa511-127">O identificador exclusivo para a intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="aa511-127">The unique identifier for the management intent.</span></span> <span data-ttu-id="aa511-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa511-128">Required.</span></span> <span data-ttu-id="aa511-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa511-129">Read-only.</span></span>|
|<span data-ttu-id="aa511-130">isGlobal</span><span class="sxs-lookup"><span data-stu-id="aa511-130">isGlobal</span></span>|<span data-ttu-id="aa511-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa511-131">Boolean</span></span>|<span data-ttu-id="aa511-132">Um sinalizador que indica se a intenção de gerenciamento é global.</span><span class="sxs-lookup"><span data-stu-id="aa511-132">A flag indicating whether the management intent is global.</span></span> <span data-ttu-id="aa511-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa511-133">Required.</span></span> <span data-ttu-id="aa511-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa511-134">Read-only.</span></span>|
|<span data-ttu-id="aa511-135">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="aa511-135">managementTemplates</span></span>|<span data-ttu-id="aa511-136">[coleção microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)</span><span class="sxs-lookup"><span data-stu-id="aa511-136">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="aa511-137">A coleção de modelos de gerenciamento associados à intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="aa511-137">The collection of management templates associated with the management intent.</span></span> <span data-ttu-id="aa511-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa511-138">Optional.</span></span> <span data-ttu-id="aa511-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa511-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa511-140">Relações</span><span class="sxs-lookup"><span data-stu-id="aa511-140">Relationships</span></span>
<span data-ttu-id="aa511-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa511-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa511-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa511-142">JSON representation</span></span>
<span data-ttu-id="aa511-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa511-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "isGlobal": "Boolean",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
