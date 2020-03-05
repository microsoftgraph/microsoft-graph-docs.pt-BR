---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3841ab8e10bb1306dcd2f7b5b3002ded0bd2fcbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491425"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="c5f79-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c5f79-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="c5f79-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c5f79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5f79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5f79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5f79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f79-107">Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.</span><span class="sxs-lookup"><span data-stu-id="c5f79-107">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="c5f79-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5f79-108">Methods</span></span>
|<span data-ttu-id="c5f79-109">Método</span><span class="sxs-lookup"><span data-stu-id="c5f79-109">Method</span></span>|<span data-ttu-id="c5f79-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5f79-110">Return Type</span></span>|<span data-ttu-id="c5f79-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f79-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5f79-112">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="c5f79-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="c5f79-113">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c5f79-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="c5f79-114">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f79-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="c5f79-115">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c5f79-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="c5f79-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c5f79-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="c5f79-117">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f79-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5f79-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5f79-118">Properties</span></span>
|<span data-ttu-id="c5f79-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5f79-119">Property</span></span>|<span data-ttu-id="c5f79-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f79-120">Type</span></span>|<span data-ttu-id="c5f79-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f79-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f79-122">id</span><span class="sxs-lookup"><span data-stu-id="c5f79-122">id</span></span>|<span data-ttu-id="c5f79-123">String</span><span class="sxs-lookup"><span data-stu-id="c5f79-123">String</span></span>|<span data-ttu-id="c5f79-124">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="c5f79-124">The relationship entity id.</span></span>|
|<span data-ttu-id="c5f79-125">targetId</span><span class="sxs-lookup"><span data-stu-id="c5f79-125">targetId</span></span>|<span data-ttu-id="c5f79-126">String</span><span class="sxs-lookup"><span data-stu-id="c5f79-126">String</span></span>|<span data-ttu-id="c5f79-127">A ID de aplicativo do aplicativo móvel do filho de destino.</span><span class="sxs-lookup"><span data-stu-id="c5f79-127">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="c5f79-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5f79-128">targetDisplayName</span></span>|<span data-ttu-id="c5f79-129">String</span><span class="sxs-lookup"><span data-stu-id="c5f79-129">String</span></span>|<span data-ttu-id="c5f79-130">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="c5f79-130">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5f79-131">Relações</span><span class="sxs-lookup"><span data-stu-id="c5f79-131">Relationships</span></span>
<span data-ttu-id="c5f79-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5f79-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5f79-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5f79-133">JSON Representation</span></span>
<span data-ttu-id="c5f79-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5f79-134">Here is a JSON representation of the resource.</span></span>
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



