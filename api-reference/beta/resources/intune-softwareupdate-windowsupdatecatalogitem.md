---
title: Tipo de recurso windowsUpdateCatalogItem
description: Entidade de item de catálogo do Windows Update
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5de85dde2c9f2b5bc68e9644b96852bdbe880de
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162164"
---
# <a name="windowsupdatecatalogitem-resource-type"></a><span data-ttu-id="1065a-103">Tipo de recurso windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="1065a-103">windowsUpdateCatalogItem resource type</span></span>

<span data-ttu-id="1065a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1065a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1065a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1065a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1065a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1065a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1065a-107">Entidade de item de catálogo do Windows Update</span><span class="sxs-lookup"><span data-stu-id="1065a-107">Windows update catalog item entity</span></span>

## <a name="methods"></a><span data-ttu-id="1065a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1065a-108">Methods</span></span>
|<span data-ttu-id="1065a-109">Método</span><span class="sxs-lookup"><span data-stu-id="1065a-109">Method</span></span>|<span data-ttu-id="1065a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1065a-110">Return Type</span></span>|<span data-ttu-id="1065a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1065a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1065a-112">Listar windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="1065a-112">List windowsUpdateCatalogItems</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|<span data-ttu-id="1065a-113">[Coleção windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1065a-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) collection</span></span>|<span data-ttu-id="1065a-114">Listar propriedades e relações dos [objetos windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1065a-114">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>|
|[<span data-ttu-id="1065a-115">Obter windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="1065a-115">Get windowsUpdateCatalogItem</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[<span data-ttu-id="1065a-116">windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="1065a-116">windowsUpdateCatalogItem</span></span>](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|<span data-ttu-id="1065a-117">Leia as propriedades e as relações do [objeto windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1065a-117">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1065a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1065a-118">Properties</span></span>
|<span data-ttu-id="1065a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1065a-119">Property</span></span>|<span data-ttu-id="1065a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1065a-120">Type</span></span>|<span data-ttu-id="1065a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1065a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1065a-122">id</span><span class="sxs-lookup"><span data-stu-id="1065a-122">id</span></span>|<span data-ttu-id="1065a-123">String</span><span class="sxs-lookup"><span data-stu-id="1065a-123">String</span></span>|<span data-ttu-id="1065a-124">A ID do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="1065a-124">The catalog item id.</span></span>|
|<span data-ttu-id="1065a-125">displayName</span><span class="sxs-lookup"><span data-stu-id="1065a-125">displayName</span></span>|<span data-ttu-id="1065a-126">String</span><span class="sxs-lookup"><span data-stu-id="1065a-126">String</span></span>|<span data-ttu-id="1065a-127">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="1065a-127">The display name for the catalog item.</span></span>|
|<span data-ttu-id="1065a-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1065a-128">releaseDateTime</span></span>|<span data-ttu-id="1065a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1065a-129">DateTimeOffset</span></span>|<span data-ttu-id="1065a-130">A data em que o item de catálogo foi lançado</span><span class="sxs-lookup"><span data-stu-id="1065a-130">The date the catalog item was released</span></span>|

## <a name="relationships"></a><span data-ttu-id="1065a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="1065a-131">Relationships</span></span>
<span data-ttu-id="1065a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1065a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1065a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1065a-133">JSON Representation</span></span>
<span data-ttu-id="1065a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1065a-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)"
}
```




