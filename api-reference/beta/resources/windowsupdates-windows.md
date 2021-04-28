---
title: tipo de recurso do windows
description: Entidade que atua como um contêiner para Windows funcionalidade.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3f7677f97db8d57e1fba74174df8cd848ad4f224
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067230"
---
# <a name="windows-resource-type"></a><span data-ttu-id="90842-103">tipo de recurso do windows</span><span class="sxs-lookup"><span data-stu-id="90842-103">windows resource type</span></span>

<span data-ttu-id="90842-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="90842-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90842-105">Entidade que atua como um contêiner para Windows funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="90842-105">Entity that acts as a container for Windows functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="90842-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90842-106">Properties</span></span>
|<span data-ttu-id="90842-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90842-107">Property</span></span>|<span data-ttu-id="90842-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90842-108">Type</span></span>|<span data-ttu-id="90842-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90842-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90842-110">id</span><span class="sxs-lookup"><span data-stu-id="90842-110">id</span></span>|<span data-ttu-id="90842-111">String</span><span class="sxs-lookup"><span data-stu-id="90842-111">String</span></span>|<span data-ttu-id="90842-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90842-112">Read-only.</span></span> <span data-ttu-id="90842-113">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="90842-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="90842-114">Relações</span><span class="sxs-lookup"><span data-stu-id="90842-114">Relationships</span></span>
|<span data-ttu-id="90842-115">Relação</span><span class="sxs-lookup"><span data-stu-id="90842-115">Relationship</span></span>|<span data-ttu-id="90842-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="90842-116">Type</span></span>|<span data-ttu-id="90842-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="90842-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90842-118">atualizações</span><span class="sxs-lookup"><span data-stu-id="90842-118">updates</span></span>|[<span data-ttu-id="90842-119">microsoft.graph.windowsUpdates.updates</span><span class="sxs-lookup"><span data-stu-id="90842-119">microsoft.graph.windowsUpdates.updates</span></span>](../resources/windowsupdates-updates.md)|<span data-ttu-id="90842-120">Entidade que atua como um contêiner para a funcionalidade do serviço de implantação Windows Update for Business.</span><span class="sxs-lookup"><span data-stu-id="90842-120">Entity that acts as a container for the functionality of the Windows Update for Business deployment service.</span></span> <span data-ttu-id="90842-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90842-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90842-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90842-122">JSON representation</span></span>
<span data-ttu-id="90842-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90842-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.windows",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windows",
  "id": "String (identifier)"
}
```

