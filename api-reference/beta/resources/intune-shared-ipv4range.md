---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4779e1090c5641d31ddafac1b47753980abf66
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255837"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="c3bcc-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="c3bcc-103">iPv4Range resource type</span></span>

<span data-ttu-id="c3bcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3bcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3bcc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bcc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bcc-107">Definição de intervalo IPv4.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-107">IPv4 Range definition.</span></span>


<span data-ttu-id="c3bcc-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c3bcc-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3bcc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3bcc-109">Properties</span></span>
|<span data-ttu-id="c3bcc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3bcc-110">Property</span></span>|<span data-ttu-id="c3bcc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3bcc-111">Type</span></span>|<span data-ttu-id="c3bcc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bcc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bcc-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c3bcc-113">lowerAddress</span></span>|<span data-ttu-id="c3bcc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bcc-114">String</span></span>|<span data-ttu-id="c3bcc-115">Endereço inferior.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-115">Lower address.</span></span>|
|<span data-ttu-id="c3bcc-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c3bcc-116">upperAddress</span></span>|<span data-ttu-id="c3bcc-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bcc-117">String</span></span>|<span data-ttu-id="c3bcc-118">Endereço superior.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3bcc-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c3bcc-119">Relationships</span></span>
<span data-ttu-id="c3bcc-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3bcc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3bcc-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3bcc-121">JSON Representation</span></span>
<span data-ttu-id="c3bcc-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3bcc-122">Here is a JSON representation of the resource.</span></span>
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




