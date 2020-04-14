---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80cf0fd5897d0ff3d1b3b3adc5343ad4c059442e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462579"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="81cd3-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="81cd3-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="81cd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81cd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81cd3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81cd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81cd3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81cd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81cd3-107">Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.</span><span class="sxs-lookup"><span data-stu-id="81cd3-107">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="81cd3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="81cd3-108">Methods</span></span>
|<span data-ttu-id="81cd3-109">Método</span><span class="sxs-lookup"><span data-stu-id="81cd3-109">Method</span></span>|<span data-ttu-id="81cd3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81cd3-110">Return Type</span></span>|<span data-ttu-id="81cd3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81cd3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81cd3-112">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="81cd3-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="81cd3-113">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="81cd3-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="81cd3-114">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="81cd3-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="81cd3-115">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="81cd3-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="81cd3-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="81cd3-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="81cd3-117">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="81cd3-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81cd3-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81cd3-118">Properties</span></span>
|<span data-ttu-id="81cd3-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81cd3-119">Property</span></span>|<span data-ttu-id="81cd3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="81cd3-120">Type</span></span>|<span data-ttu-id="81cd3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="81cd3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81cd3-122">id</span><span class="sxs-lookup"><span data-stu-id="81cd3-122">id</span></span>|<span data-ttu-id="81cd3-123">String</span><span class="sxs-lookup"><span data-stu-id="81cd3-123">String</span></span>|<span data-ttu-id="81cd3-124">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="81cd3-124">The relationship entity id.</span></span>|
|<span data-ttu-id="81cd3-125">targetId</span><span class="sxs-lookup"><span data-stu-id="81cd3-125">targetId</span></span>|<span data-ttu-id="81cd3-126">String</span><span class="sxs-lookup"><span data-stu-id="81cd3-126">String</span></span>|<span data-ttu-id="81cd3-127">A ID de aplicativo do aplicativo móvel do filho de destino.</span><span class="sxs-lookup"><span data-stu-id="81cd3-127">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="81cd3-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="81cd3-128">targetDisplayName</span></span>|<span data-ttu-id="81cd3-129">String</span><span class="sxs-lookup"><span data-stu-id="81cd3-129">String</span></span>|<span data-ttu-id="81cd3-130">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="81cd3-130">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81cd3-131">Relações</span><span class="sxs-lookup"><span data-stu-id="81cd3-131">Relationships</span></span>
<span data-ttu-id="81cd3-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81cd3-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81cd3-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81cd3-133">JSON Representation</span></span>
<span data-ttu-id="81cd3-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81cd3-134">Here is a JSON representation of the resource.</span></span>
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



