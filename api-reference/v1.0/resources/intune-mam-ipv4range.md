---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465521"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="36207-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="36207-103">iPv4Range resource type</span></span>

> <span data-ttu-id="36207-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36207-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36207-105">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="36207-105">IPv4 Range definition.</span></span>


<span data-ttu-id="36207-106">Herda de [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="36207-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36207-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36207-107">Properties</span></span>
|<span data-ttu-id="36207-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36207-108">Property</span></span>|<span data-ttu-id="36207-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="36207-109">Type</span></span>|<span data-ttu-id="36207-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="36207-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36207-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="36207-111">lowerAddress</span></span>|<span data-ttu-id="36207-112">String</span><span class="sxs-lookup"><span data-stu-id="36207-112">String</span></span>|<span data-ttu-id="36207-113">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="36207-113">Lower address.</span></span>|
|<span data-ttu-id="36207-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="36207-114">upperAddress</span></span>|<span data-ttu-id="36207-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36207-115">String</span></span>|<span data-ttu-id="36207-116">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="36207-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36207-117">Relações</span><span class="sxs-lookup"><span data-stu-id="36207-117">Relationships</span></span>
<span data-ttu-id="36207-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="36207-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36207-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36207-119">JSON Representation</span></span>
<span data-ttu-id="36207-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36207-120">Here is a JSON representation of the resource.</span></span>
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



