---
title: tipo de recurso de operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
ms.openlocfilehash: af140bf2a5d889b66d45460465e47c466bb2160b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035197"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="5f62a-103">tipo de recurso de operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="5f62a-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="5f62a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f62a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f62a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f62a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f62a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5f62a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f62a-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5f62a-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="5f62a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f62a-108">Properties</span></span>
|<span data-ttu-id="5f62a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f62a-109">Property</span></span>|<span data-ttu-id="5f62a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f62a-110">Type</span></span>|<span data-ttu-id="5f62a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f62a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f62a-112">description</span><span class="sxs-lookup"><span data-stu-id="5f62a-112">description</span></span>|<span data-ttu-id="5f62a-113">String</span><span class="sxs-lookup"><span data-stu-id="5f62a-113">String</span></span>|<span data-ttu-id="5f62a-114">A descrição deste intervalo (por exemplo, válido 1702 compilações)</span><span class="sxs-lookup"><span data-stu-id="5f62a-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="5f62a-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="5f62a-115">lowestVersion</span></span>|<span data-ttu-id="5f62a-116">String</span><span class="sxs-lookup"><span data-stu-id="5f62a-116">String</span></span>|<span data-ttu-id="5f62a-117">A menor inclusive versão que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5f62a-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="5f62a-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="5f62a-118">highestVersion</span></span>|<span data-ttu-id="5f62a-119">String</span><span class="sxs-lookup"><span data-stu-id="5f62a-119">String</span></span>|<span data-ttu-id="5f62a-120">A versão inclusive maior que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5f62a-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f62a-121">Relações</span><span class="sxs-lookup"><span data-stu-id="5f62a-121">Relationships</span></span>
<span data-ttu-id="5f62a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f62a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f62a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f62a-123">JSON Representation</span></span>
<span data-ttu-id="5f62a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f62a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





