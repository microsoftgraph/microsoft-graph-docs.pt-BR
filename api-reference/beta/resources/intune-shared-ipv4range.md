---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
ms.openlocfilehash: eae240d185a6cf0dc2fc7d0d83194dc9f3f6f00d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314767"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="bc5ef-103">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="bc5ef-103">iPv4Range resource type</span></span>

> <span data-ttu-id="bc5ef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc5ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc5ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc5ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc5ef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc5ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc5ef-107">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="bc5ef-107">IP V4 range</span></span>

<span data-ttu-id="bc5ef-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bc5ef-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc5ef-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc5ef-109">Properties</span></span>
|<span data-ttu-id="bc5ef-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc5ef-110">Property</span></span>|<span data-ttu-id="bc5ef-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc5ef-111">Type</span></span>|<span data-ttu-id="bc5ef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc5ef-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="bc5ef-113">lowerAddress</span></span>|<span data-ttu-id="bc5ef-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc5ef-114">String</span></span>|<span data-ttu-id="bc5ef-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="bc5ef-115">Lower IP Address</span></span>|
|<span data-ttu-id="bc5ef-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="bc5ef-116">upperAddress</span></span>|<span data-ttu-id="bc5ef-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc5ef-117">String</span></span>|<span data-ttu-id="bc5ef-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="bc5ef-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc5ef-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bc5ef-119">Relationships</span></span>
<span data-ttu-id="bc5ef-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc5ef-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc5ef-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc5ef-121">JSON Representation</span></span>
<span data-ttu-id="bc5ef-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc5ef-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



