---
title: tipo de recurso mobileAppRelationship
description: Descreve uma relação entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d09d9d7604699ee89b6dccc0f2f980cef26225e7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790863"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="f4b93-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="f4b93-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="f4b93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4b93-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4b93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4b93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4b93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b93-107">Descreve uma relação entre dois aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="f4b93-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="f4b93-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f4b93-108">Methods</span></span>
|<span data-ttu-id="f4b93-109">Método</span><span class="sxs-lookup"><span data-stu-id="f4b93-109">Method</span></span>|<span data-ttu-id="f4b93-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4b93-110">Return Type</span></span>|<span data-ttu-id="f4b93-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b93-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4b93-112">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="f4b93-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="f4b93-113">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="f4b93-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="f4b93-114">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="f4b93-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="f4b93-115">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="f4b93-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="f4b93-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="f4b93-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="f4b93-117">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="f4b93-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4b93-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4b93-118">Properties</span></span>
|<span data-ttu-id="f4b93-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4b93-119">Property</span></span>|<span data-ttu-id="f4b93-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4b93-120">Type</span></span>|<span data-ttu-id="f4b93-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b93-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b93-122">id</span><span class="sxs-lookup"><span data-stu-id="f4b93-122">id</span></span>|<span data-ttu-id="f4b93-123">String</span><span class="sxs-lookup"><span data-stu-id="f4b93-123">String</span></span>|<span data-ttu-id="f4b93-124">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="f4b93-124">The relationship entity id.</span></span>|
|<span data-ttu-id="f4b93-125">targetId</span><span class="sxs-lookup"><span data-stu-id="f4b93-125">targetId</span></span>|<span data-ttu-id="f4b93-126">String</span><span class="sxs-lookup"><span data-stu-id="f4b93-126">String</span></span>|<span data-ttu-id="f4b93-127">A ID de aplicativo do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="f4b93-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="f4b93-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4b93-128">targetDisplayName</span></span>|<span data-ttu-id="f4b93-129">String</span><span class="sxs-lookup"><span data-stu-id="f4b93-129">String</span></span>|<span data-ttu-id="f4b93-130">O nome de exibição do aplicativo móvel de destino.</span><span class="sxs-lookup"><span data-stu-id="f4b93-130">The target mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b93-131">Relações</span><span class="sxs-lookup"><span data-stu-id="f4b93-131">Relationships</span></span>
<span data-ttu-id="f4b93-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f4b93-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4b93-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4b93-133">JSON Representation</span></span>
<span data-ttu-id="f4b93-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4b93-134">Here is a JSON representation of the resource.</span></span>
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
  "targetDisplayName": "String"
}
```



