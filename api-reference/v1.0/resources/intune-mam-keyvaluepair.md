---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd0f9c6e17d1550e4b2584200239ff303ba91232
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038112"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="c2636-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="c2636-103">keyValuePair resource type</span></span>

> <span data-ttu-id="c2636-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2636-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2636-105">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="c2636-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="c2636-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2636-106">Properties</span></span>
|<span data-ttu-id="c2636-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2636-107">Property</span></span>|<span data-ttu-id="c2636-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2636-108">Type</span></span>|<span data-ttu-id="c2636-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2636-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2636-110">name</span><span class="sxs-lookup"><span data-stu-id="c2636-110">name</span></span>|<span data-ttu-id="c2636-111">String</span><span class="sxs-lookup"><span data-stu-id="c2636-111">String</span></span>|<span data-ttu-id="c2636-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="c2636-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="c2636-113">value</span><span class="sxs-lookup"><span data-stu-id="c2636-113">value</span></span>|<span data-ttu-id="c2636-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2636-114">String</span></span>|<span data-ttu-id="c2636-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="c2636-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2636-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c2636-116">Relationships</span></span>
<span data-ttu-id="c2636-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2636-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2636-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2636-118">JSON Representation</span></span>
<span data-ttu-id="c2636-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2636-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



