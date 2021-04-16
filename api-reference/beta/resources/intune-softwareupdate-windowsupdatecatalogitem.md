---
title: Tipo de recurso windowsUpdateCatalogItem
description: Entidade de item do catálogo de atualizações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6faffa482a2fc79e653eedf8a70a041f264d7d49
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863608"
---
# <a name="windowsupdatecatalogitem-resource-type"></a><span data-ttu-id="a08c2-103">Tipo de recurso windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="a08c2-103">windowsUpdateCatalogItem resource type</span></span>

<span data-ttu-id="a08c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a08c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a08c2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a08c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a08c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a08c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a08c2-107">Entidade de item do catálogo de atualizações do Windows</span><span class="sxs-lookup"><span data-stu-id="a08c2-107">Windows update catalog item entity</span></span>

## <a name="methods"></a><span data-ttu-id="a08c2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a08c2-108">Methods</span></span>
|<span data-ttu-id="a08c2-109">Método</span><span class="sxs-lookup"><span data-stu-id="a08c2-109">Method</span></span>|<span data-ttu-id="a08c2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a08c2-110">Return Type</span></span>|<span data-ttu-id="a08c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a08c2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a08c2-112">Listar windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="a08c2-112">List windowsUpdateCatalogItems</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|<span data-ttu-id="a08c2-113">[Coleção windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="a08c2-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) collection</span></span>|<span data-ttu-id="a08c2-114">Listar propriedades e relações dos [objetos windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="a08c2-114">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>|
|[<span data-ttu-id="a08c2-115">Obter windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="a08c2-115">Get windowsUpdateCatalogItem</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[<span data-ttu-id="a08c2-116">windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="a08c2-116">windowsUpdateCatalogItem</span></span>](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|<span data-ttu-id="a08c2-117">Ler propriedades e relações do [objeto windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="a08c2-117">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a08c2-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a08c2-118">Properties</span></span>
|<span data-ttu-id="a08c2-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a08c2-119">Property</span></span>|<span data-ttu-id="a08c2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a08c2-120">Type</span></span>|<span data-ttu-id="a08c2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a08c2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a08c2-122">id</span><span class="sxs-lookup"><span data-stu-id="a08c2-122">id</span></span>|<span data-ttu-id="a08c2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a08c2-123">String</span></span>|<span data-ttu-id="a08c2-124">A ID do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="a08c2-124">The catalog item id.</span></span>|
|<span data-ttu-id="a08c2-125">displayName</span><span class="sxs-lookup"><span data-stu-id="a08c2-125">displayName</span></span>|<span data-ttu-id="a08c2-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a08c2-126">String</span></span>|<span data-ttu-id="a08c2-127">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="a08c2-127">The display name for the catalog item.</span></span>|
|<span data-ttu-id="a08c2-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="a08c2-128">releaseDateTime</span></span>|<span data-ttu-id="a08c2-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a08c2-129">DateTimeOffset</span></span>|<span data-ttu-id="a08c2-130">A data em que o item de catálogo foi lançado</span><span class="sxs-lookup"><span data-stu-id="a08c2-130">The date the catalog item was released</span></span>|
|<span data-ttu-id="a08c2-131">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="a08c2-131">endOfSupportDate</span></span>|<span data-ttu-id="a08c2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a08c2-132">DateTimeOffset</span></span>|<span data-ttu-id="a08c2-133">A última data com suporte para um item de catálogo</span><span class="sxs-lookup"><span data-stu-id="a08c2-133">The last supported date for a catalog item</span></span>|

## <a name="relationships"></a><span data-ttu-id="a08c2-134">Relações</span><span class="sxs-lookup"><span data-stu-id="a08c2-134">Relationships</span></span>
<span data-ttu-id="a08c2-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a08c2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a08c2-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a08c2-136">JSON Representation</span></span>
<span data-ttu-id="a08c2-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a08c2-137">Here is a JSON representation of the resource.</span></span>
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
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```




