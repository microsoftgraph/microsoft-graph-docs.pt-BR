---
title: tipo de recurso de operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331161"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="fac78-103">tipo de recurso de operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="fac78-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="fac78-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fac78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fac78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fac78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fac78-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fac78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fac78-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="fac78-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="fac78-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fac78-108">Properties</span></span>
|<span data-ttu-id="fac78-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fac78-109">Property</span></span>|<span data-ttu-id="fac78-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fac78-110">Type</span></span>|<span data-ttu-id="fac78-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fac78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fac78-112">description</span><span class="sxs-lookup"><span data-stu-id="fac78-112">description</span></span>|<span data-ttu-id="fac78-113">String</span><span class="sxs-lookup"><span data-stu-id="fac78-113">String</span></span>|<span data-ttu-id="fac78-114">A descrição deste intervalo (por exemplo, válido 1702 compilações)</span><span class="sxs-lookup"><span data-stu-id="fac78-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="fac78-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="fac78-115">lowestVersion</span></span>|<span data-ttu-id="fac78-116">String</span><span class="sxs-lookup"><span data-stu-id="fac78-116">String</span></span>|<span data-ttu-id="fac78-117">A menor inclusive versão que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="fac78-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="fac78-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="fac78-118">highestVersion</span></span>|<span data-ttu-id="fac78-119">String</span><span class="sxs-lookup"><span data-stu-id="fac78-119">String</span></span>|<span data-ttu-id="fac78-120">A versão inclusive maior que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="fac78-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fac78-121">Relações</span><span class="sxs-lookup"><span data-stu-id="fac78-121">Relationships</span></span>
<span data-ttu-id="fac78-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fac78-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fac78-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fac78-123">JSON Representation</span></span>
<span data-ttu-id="fac78-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fac78-124">Here is a JSON representation of the resource.</span></span>
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





