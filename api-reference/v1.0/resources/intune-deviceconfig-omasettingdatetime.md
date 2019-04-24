---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585395"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0d3a8-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="0d3a8-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="0d3a8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d3a8-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="0d3a8-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0d3a8-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d3a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d3a8-107">Properties</span></span>
|<span data-ttu-id="0d3a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d3a8-108">Property</span></span>|<span data-ttu-id="0d3a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d3a8-109">Type</span></span>|<span data-ttu-id="0d3a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d3a8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0d3a8-111">displayName</span></span>|<span data-ttu-id="0d3a8-112">String</span><span class="sxs-lookup"><span data-stu-id="0d3a8-112">String</span></span>|<span data-ttu-id="0d3a8-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-113">Display Name.</span></span> <span data-ttu-id="0d3a8-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0d3a8-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0d3a8-115">description</span><span class="sxs-lookup"><span data-stu-id="0d3a8-115">description</span></span>|<span data-ttu-id="0d3a8-116">String</span><span class="sxs-lookup"><span data-stu-id="0d3a8-116">String</span></span>|<span data-ttu-id="0d3a8-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-117">Description.</span></span> <span data-ttu-id="0d3a8-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0d3a8-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0d3a8-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0d3a8-119">omaUri</span></span>|<span data-ttu-id="0d3a8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d3a8-120">String</span></span>|<span data-ttu-id="0d3a8-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-121">OMA.</span></span> <span data-ttu-id="0d3a8-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0d3a8-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0d3a8-123">value</span><span class="sxs-lookup"><span data-stu-id="0d3a8-123">value</span></span>|<span data-ttu-id="0d3a8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d3a8-124">DateTimeOffset</span></span>|<span data-ttu-id="0d3a8-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d3a8-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0d3a8-126">Relationships</span></span>
<span data-ttu-id="0d3a8-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0d3a8-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d3a8-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d3a8-128">JSON Representation</span></span>
<span data-ttu-id="0d3a8-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d3a8-129">Here is a JSON representation of the resource.</span></span>
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



