---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7bdde3831a3634dce25e562ea1d1a332c18fac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984422"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="0af5f-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="0af5f-103">iPv6Range resource type</span></span>

<span data-ttu-id="0af5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0af5f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0af5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0af5f-106">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="0af5f-106">IPv6 Range definition.</span></span>


<span data-ttu-id="0af5f-107">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0af5f-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0af5f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0af5f-108">Properties</span></span>
|<span data-ttu-id="0af5f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0af5f-109">Property</span></span>|<span data-ttu-id="0af5f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0af5f-110">Type</span></span>|<span data-ttu-id="0af5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0af5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af5f-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="0af5f-112">lowerAddress</span></span>|<span data-ttu-id="0af5f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0af5f-113">String</span></span>|<span data-ttu-id="0af5f-114">Endereço inferior</span><span class="sxs-lookup"><span data-stu-id="0af5f-114">Lower address</span></span>|
|<span data-ttu-id="0af5f-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="0af5f-115">upperAddress</span></span>|<span data-ttu-id="0af5f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0af5f-116">String</span></span>|<span data-ttu-id="0af5f-117">Endereço superior</span><span class="sxs-lookup"><span data-stu-id="0af5f-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="0af5f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0af5f-118">Relationships</span></span>
<span data-ttu-id="0af5f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0af5f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af5f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0af5f-120">JSON Representation</span></span>
<span data-ttu-id="0af5f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0af5f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```









