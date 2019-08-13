---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97ff0d0331523a93d57c9f14cd8bb45910b9cdb2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331851"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="6e9f6-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="6e9f6-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="6e9f6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e9f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e9f6-106">Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="6e9f6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e9f6-107">Methods</span></span>
|<span data-ttu-id="6e9f6-108">Método</span><span class="sxs-lookup"><span data-stu-id="6e9f6-108">Method</span></span>|<span data-ttu-id="6e9f6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e9f6-109">Return Type</span></span>|<span data-ttu-id="6e9f6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e9f6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e9f6-111">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="6e9f6-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="6e9f6-112">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="6e9f6-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="6e9f6-113">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="6e9f6-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="6e9f6-114">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="6e9f6-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="6e9f6-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="6e9f6-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="6e9f6-116">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="6e9f6-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e9f6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e9f6-117">Properties</span></span>
|<span data-ttu-id="6e9f6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e9f6-118">Property</span></span>|<span data-ttu-id="6e9f6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e9f6-119">Type</span></span>|<span data-ttu-id="6e9f6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e9f6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e9f6-121">id</span><span class="sxs-lookup"><span data-stu-id="6e9f6-121">id</span></span>|<span data-ttu-id="6e9f6-122">String</span><span class="sxs-lookup"><span data-stu-id="6e9f6-122">String</span></span>|<span data-ttu-id="6e9f6-123">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-123">The relationship entity id.</span></span>|
|<span data-ttu-id="6e9f6-124">targetId</span><span class="sxs-lookup"><span data-stu-id="6e9f6-124">targetId</span></span>|<span data-ttu-id="6e9f6-125">String</span><span class="sxs-lookup"><span data-stu-id="6e9f6-125">String</span></span>|<span data-ttu-id="6e9f6-126">A ID de aplicativo do aplicativo móvel do filho de destino.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="6e9f6-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e9f6-127">targetDisplayName</span></span>|<span data-ttu-id="6e9f6-128">String</span><span class="sxs-lookup"><span data-stu-id="6e9f6-128">String</span></span>|<span data-ttu-id="6e9f6-129">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e9f6-130">Relações</span><span class="sxs-lookup"><span data-stu-id="6e9f6-130">Relationships</span></span>
<span data-ttu-id="6e9f6-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e9f6-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e9f6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e9f6-132">JSON Representation</span></span>
<span data-ttu-id="6e9f6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e9f6-133">Here is a JSON representation of the resource.</span></span>
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



