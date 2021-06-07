---
title: Tipo de recurso iPv4Range
description: Definição de Intervalo IPv4.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e3ad2761050ec3bf0a26a2da5e7faf83a8e5523
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752781"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="c76a2-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="c76a2-103">iPv4Range resource type</span></span>

<span data-ttu-id="c76a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c76a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c76a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c76a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c76a2-106">Definição de Intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="c76a2-106">IPv4 Range definition.</span></span>


<span data-ttu-id="c76a2-107">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c76a2-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c76a2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c76a2-108">Properties</span></span>
|<span data-ttu-id="c76a2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c76a2-109">Property</span></span>|<span data-ttu-id="c76a2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76a2-110">Type</span></span>|<span data-ttu-id="c76a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c76a2-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c76a2-112">lowerAddress</span></span>|<span data-ttu-id="c76a2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76a2-113">String</span></span>|<span data-ttu-id="c76a2-114">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="c76a2-114">Lower address.</span></span>|
|<span data-ttu-id="c76a2-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c76a2-115">upperAddress</span></span>|<span data-ttu-id="c76a2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76a2-116">String</span></span>|<span data-ttu-id="c76a2-117">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="c76a2-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c76a2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c76a2-118">Relationships</span></span>
<span data-ttu-id="c76a2-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c76a2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c76a2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c76a2-120">JSON Representation</span></span>
<span data-ttu-id="c76a2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c76a2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




