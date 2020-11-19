---
title: tipo de recurso mobileAppRelationship
description: Descreve uma relação entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22af70876075aa12b5493cfa413c79bd2c71c7cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217190"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="d6321-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="d6321-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="d6321-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6321-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6321-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6321-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6321-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6321-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6321-107">Descreve uma relação entre dois aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="d6321-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="d6321-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6321-108">Methods</span></span>
|<span data-ttu-id="d6321-109">Método</span><span class="sxs-lookup"><span data-stu-id="d6321-109">Method</span></span>|<span data-ttu-id="d6321-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6321-110">Return Type</span></span>|<span data-ttu-id="d6321-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6321-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6321-112">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="d6321-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="d6321-113">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d6321-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="d6321-114">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="d6321-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="d6321-115">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="d6321-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="d6321-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="d6321-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="d6321-117">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="d6321-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6321-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6321-118">Properties</span></span>
|<span data-ttu-id="d6321-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6321-119">Property</span></span>|<span data-ttu-id="d6321-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6321-120">Type</span></span>|<span data-ttu-id="d6321-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6321-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6321-122">id</span><span class="sxs-lookup"><span data-stu-id="d6321-122">id</span></span>|<span data-ttu-id="d6321-123">String</span><span class="sxs-lookup"><span data-stu-id="d6321-123">String</span></span>|<span data-ttu-id="d6321-124">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="d6321-124">The relationship entity id.</span></span>|
|<span data-ttu-id="d6321-125">targetId</span><span class="sxs-lookup"><span data-stu-id="d6321-125">targetId</span></span>|<span data-ttu-id="d6321-126">String</span><span class="sxs-lookup"><span data-stu-id="d6321-126">String</span></span>|<span data-ttu-id="d6321-127">A ID de aplicativo do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d6321-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="d6321-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6321-128">targetDisplayName</span></span>|<span data-ttu-id="d6321-129">String</span><span class="sxs-lookup"><span data-stu-id="d6321-129">String</span></span>|<span data-ttu-id="d6321-130">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d6321-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="d6321-131">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="d6321-131">targetDisplayVersion</span></span>|<span data-ttu-id="d6321-132">String</span><span class="sxs-lookup"><span data-stu-id="d6321-132">String</span></span>|<span data-ttu-id="d6321-133">A versão de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d6321-133">The target mobile app's display version.</span></span>|
|<span data-ttu-id="d6321-134">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="d6321-134">targetPublisher</span></span>|<span data-ttu-id="d6321-135">String</span><span class="sxs-lookup"><span data-stu-id="d6321-135">String</span></span>|<span data-ttu-id="d6321-136">O fornecedor do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="d6321-136">The target mobile app's publisher.</span></span>|
|<span data-ttu-id="d6321-137">targetType</span><span class="sxs-lookup"><span data-stu-id="d6321-137">targetType</span></span>|[<span data-ttu-id="d6321-138">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="d6321-138">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="d6321-139">O tipo de relação que indica se o destino é um pai ou filho.</span><span class="sxs-lookup"><span data-stu-id="d6321-139">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="d6321-140">Os valores possíveis são: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="d6321-140">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6321-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d6321-141">Relationships</span></span>
<span data-ttu-id="d6321-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6321-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6321-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6321-143">JSON Representation</span></span>
<span data-ttu-id="d6321-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6321-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```




