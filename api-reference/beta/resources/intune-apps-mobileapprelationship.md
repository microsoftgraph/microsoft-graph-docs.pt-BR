---
title: tipo de recurso mobileAppRelationship
description: Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c871ba51733195947243fa9b22824156108f5eb7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949882"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="8dfe3-103">tipo de recurso mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="8dfe3-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="8dfe3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dfe3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dfe3-106">Descreve o relacionamento de um aplicativo móvel filho para seu aplicativo móvel pai.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="8dfe3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8dfe3-107">Methods</span></span>
|<span data-ttu-id="8dfe3-108">Método</span><span class="sxs-lookup"><span data-stu-id="8dfe3-108">Method</span></span>|<span data-ttu-id="8dfe3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8dfe3-109">Return Type</span></span>|<span data-ttu-id="8dfe3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dfe3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8dfe3-111">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="8dfe3-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="8dfe3-112">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="8dfe3-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="8dfe3-113">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="8dfe3-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="8dfe3-114">Obter mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="8dfe3-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="8dfe3-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="8dfe3-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="8dfe3-116">Leia as propriedades e as relações do objeto [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="8dfe3-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dfe3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dfe3-117">Properties</span></span>
|<span data-ttu-id="8dfe3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dfe3-118">Property</span></span>|<span data-ttu-id="8dfe3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dfe3-119">Type</span></span>|<span data-ttu-id="8dfe3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dfe3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dfe3-121">id</span><span class="sxs-lookup"><span data-stu-id="8dfe3-121">id</span></span>|<span data-ttu-id="8dfe3-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dfe3-122">String</span></span>|<span data-ttu-id="8dfe3-123">A ID da entidade de relação.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-123">The relationship entity id.</span></span>|
|<span data-ttu-id="8dfe3-124">targetId</span><span class="sxs-lookup"><span data-stu-id="8dfe3-124">targetId</span></span>|<span data-ttu-id="8dfe3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dfe3-125">String</span></span>|<span data-ttu-id="8dfe3-126">A ID de aplicativo do aplicativo móvel do filho de destino.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="8dfe3-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="8dfe3-127">targetDisplayName</span></span>|<span data-ttu-id="8dfe3-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dfe3-128">String</span></span>|<span data-ttu-id="8dfe3-129">O nome de exibição do aplicativo móvel filho de destino.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dfe3-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8dfe3-130">Relationships</span></span>
<span data-ttu-id="8dfe3-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8dfe3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dfe3-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dfe3-132">JSON Representation</span></span>
<span data-ttu-id="8dfe3-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dfe3-133">Here is a JSON representation of the resource.</span></span>
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




