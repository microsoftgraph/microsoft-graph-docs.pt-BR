---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c30c9a272029fc681a383772b2467dc6fb67af88
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359023"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="14fc6-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="14fc6-103">resourceAction resource type</span></span>

> <span data-ttu-id="14fc6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14fc6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14fc6-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14fc6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="14fc6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14fc6-106">Properties</span></span>
|<span data-ttu-id="14fc6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14fc6-107">Property</span></span>|<span data-ttu-id="14fc6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14fc6-108">Type</span></span>|<span data-ttu-id="14fc6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14fc6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14fc6-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="14fc6-110">allowedResourceActions</span></span>|<span data-ttu-id="14fc6-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14fc6-111">String collection</span></span>|<span data-ttu-id="14fc6-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="14fc6-112">Allowed Actions</span></span>|
|<span data-ttu-id="14fc6-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="14fc6-113">notAllowedResourceActions</span></span>|<span data-ttu-id="14fc6-114">String collection</span><span class="sxs-lookup"><span data-stu-id="14fc6-114">String collection</span></span>|<span data-ttu-id="14fc6-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="14fc6-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="14fc6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="14fc6-116">Relationships</span></span>
<span data-ttu-id="14fc6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14fc6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14fc6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14fc6-118">JSON Representation</span></span>
<span data-ttu-id="14fc6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14fc6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




