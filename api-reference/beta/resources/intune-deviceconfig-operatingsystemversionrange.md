---
title: tipo de recurso de operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398524"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="7a418-103">tipo de recurso de operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="7a418-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="7a418-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a418-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a418-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a418-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a418-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7a418-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a418-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="7a418-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="7a418-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a418-108">Properties</span></span>
|<span data-ttu-id="7a418-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a418-109">Property</span></span>|<span data-ttu-id="7a418-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a418-110">Type</span></span>|<span data-ttu-id="7a418-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a418-112">description</span><span class="sxs-lookup"><span data-stu-id="7a418-112">description</span></span>|<span data-ttu-id="7a418-113">String</span><span class="sxs-lookup"><span data-stu-id="7a418-113">String</span></span>|<span data-ttu-id="7a418-114">A descrição deste intervalo (por exemplo, válido 1702 compilações)</span><span class="sxs-lookup"><span data-stu-id="7a418-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="7a418-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="7a418-115">lowestVersion</span></span>|<span data-ttu-id="7a418-116">String</span><span class="sxs-lookup"><span data-stu-id="7a418-116">String</span></span>|<span data-ttu-id="7a418-117">A menor inclusive versão que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7a418-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="7a418-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="7a418-118">highestVersion</span></span>|<span data-ttu-id="7a418-119">String</span><span class="sxs-lookup"><span data-stu-id="7a418-119">String</span></span>|<span data-ttu-id="7a418-120">A versão inclusive maior que contém esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7a418-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a418-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7a418-121">Relationships</span></span>
<span data-ttu-id="7a418-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a418-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a418-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a418-123">JSON Representation</span></span>
<span data-ttu-id="7a418-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a418-124">Here is a JSON representation of the resource.</span></span>
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




