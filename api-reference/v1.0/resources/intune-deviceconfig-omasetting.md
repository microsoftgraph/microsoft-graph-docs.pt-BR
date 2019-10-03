---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c1b464d8947bfa0125ba7edc9991b7bc6f34296
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367382"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="b12ad-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="b12ad-103">omaSetting resource type</span></span>

> <span data-ttu-id="b12ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b12ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b12ad-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b12ad-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b12ad-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b12ad-106">Properties</span></span>
|<span data-ttu-id="b12ad-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b12ad-107">Property</span></span>|<span data-ttu-id="b12ad-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b12ad-108">Type</span></span>|<span data-ttu-id="b12ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b12ad-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b12ad-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b12ad-110">displayName</span></span>|<span data-ttu-id="b12ad-111">String</span><span class="sxs-lookup"><span data-stu-id="b12ad-111">String</span></span>|<span data-ttu-id="b12ad-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b12ad-112">Display Name.</span></span>|
|<span data-ttu-id="b12ad-113">descrição</span><span class="sxs-lookup"><span data-stu-id="b12ad-113">description</span></span>|<span data-ttu-id="b12ad-114">String</span><span class="sxs-lookup"><span data-stu-id="b12ad-114">String</span></span>|<span data-ttu-id="b12ad-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b12ad-115">Description.</span></span>|
|<span data-ttu-id="b12ad-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="b12ad-116">omaUri</span></span>|<span data-ttu-id="b12ad-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b12ad-117">String</span></span>|<span data-ttu-id="b12ad-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="b12ad-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b12ad-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b12ad-119">Relationships</span></span>
<span data-ttu-id="b12ad-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b12ad-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b12ad-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b12ad-121">JSON Representation</span></span>
<span data-ttu-id="b12ad-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b12ad-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




