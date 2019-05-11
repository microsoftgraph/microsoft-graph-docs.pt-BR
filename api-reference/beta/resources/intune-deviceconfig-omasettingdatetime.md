---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9d58c6fdbba9f4a2fcceaa5d0e2964f0666c571
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950918"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="59b15-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="59b15-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="59b15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59b15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59b15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59b15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59b15-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="59b15-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="59b15-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="59b15-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59b15-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59b15-108">Properties</span></span>
|<span data-ttu-id="59b15-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59b15-109">Property</span></span>|<span data-ttu-id="59b15-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="59b15-110">Type</span></span>|<span data-ttu-id="59b15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="59b15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59b15-112">displayName</span><span class="sxs-lookup"><span data-stu-id="59b15-112">displayName</span></span>|<span data-ttu-id="59b15-113">String</span><span class="sxs-lookup"><span data-stu-id="59b15-113">String</span></span>|<span data-ttu-id="59b15-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="59b15-114">Display Name.</span></span> <span data-ttu-id="59b15-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="59b15-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59b15-116">description</span><span class="sxs-lookup"><span data-stu-id="59b15-116">description</span></span>|<span data-ttu-id="59b15-117">String</span><span class="sxs-lookup"><span data-stu-id="59b15-117">String</span></span>|<span data-ttu-id="59b15-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="59b15-118">Description.</span></span> <span data-ttu-id="59b15-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="59b15-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59b15-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="59b15-120">omaUri</span></span>|<span data-ttu-id="59b15-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59b15-121">String</span></span>|<span data-ttu-id="59b15-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="59b15-122">OMA.</span></span> <span data-ttu-id="59b15-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="59b15-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59b15-124">value</span><span class="sxs-lookup"><span data-stu-id="59b15-124">value</span></span>|<span data-ttu-id="59b15-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59b15-125">DateTimeOffset</span></span>|<span data-ttu-id="59b15-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="59b15-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59b15-127">Relações</span><span class="sxs-lookup"><span data-stu-id="59b15-127">Relationships</span></span>
<span data-ttu-id="59b15-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59b15-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59b15-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59b15-129">JSON Representation</span></span>
<span data-ttu-id="59b15-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59b15-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```




