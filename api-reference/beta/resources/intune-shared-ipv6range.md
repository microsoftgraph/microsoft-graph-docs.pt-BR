---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a1e9e9a860783cd3598e10c2b46c46b1c6e97db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527390"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="fd256-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="fd256-103">iPv6Range resource type</span></span>

<span data-ttu-id="fd256-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fd256-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd256-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd256-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd256-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd256-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd256-107">Definição de intervalo IPv6.</span><span class="sxs-lookup"><span data-stu-id="fd256-107">IPv6 Range definition.</span></span>


<span data-ttu-id="fd256-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fd256-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd256-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd256-109">Properties</span></span>
|<span data-ttu-id="fd256-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd256-110">Property</span></span>|<span data-ttu-id="fd256-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd256-111">Type</span></span>|<span data-ttu-id="fd256-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd256-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd256-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="fd256-113">lowerAddress</span></span>|<span data-ttu-id="fd256-114">String</span><span class="sxs-lookup"><span data-stu-id="fd256-114">String</span></span>|<span data-ttu-id="fd256-115">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="fd256-115">Lower address.</span></span>|
|<span data-ttu-id="fd256-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="fd256-116">upperAddress</span></span>|<span data-ttu-id="fd256-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd256-117">String</span></span>|<span data-ttu-id="fd256-118">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="fd256-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd256-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fd256-119">Relationships</span></span>
<span data-ttu-id="fd256-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd256-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd256-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd256-121">JSON Representation</span></span>
<span data-ttu-id="fd256-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd256-122">Here is a JSON representation of the resource.</span></span>
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



