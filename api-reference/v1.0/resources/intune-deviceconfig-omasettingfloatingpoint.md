---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2f397d309f2199458595e3ed7d5cd4a204a1874
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359926"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="95914-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="95914-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="95914-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95914-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95914-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="95914-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="95914-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95914-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95914-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95914-107">Properties</span></span>
|<span data-ttu-id="95914-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95914-108">Property</span></span>|<span data-ttu-id="95914-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="95914-109">Type</span></span>|<span data-ttu-id="95914-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95914-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95914-111">displayName</span><span class="sxs-lookup"><span data-stu-id="95914-111">displayName</span></span>|<span data-ttu-id="95914-112">String</span><span class="sxs-lookup"><span data-stu-id="95914-112">String</span></span>|<span data-ttu-id="95914-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="95914-113">Display Name.</span></span> <span data-ttu-id="95914-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95914-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95914-115">descrição</span><span class="sxs-lookup"><span data-stu-id="95914-115">description</span></span>|<span data-ttu-id="95914-116">String</span><span class="sxs-lookup"><span data-stu-id="95914-116">String</span></span>|<span data-ttu-id="95914-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="95914-117">Description.</span></span> <span data-ttu-id="95914-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95914-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95914-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="95914-119">omaUri</span></span>|<span data-ttu-id="95914-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95914-120">String</span></span>|<span data-ttu-id="95914-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="95914-121">OMA.</span></span> <span data-ttu-id="95914-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95914-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95914-123">value</span><span class="sxs-lookup"><span data-stu-id="95914-123">value</span></span>|<span data-ttu-id="95914-124">Single</span><span class="sxs-lookup"><span data-stu-id="95914-124">Single</span></span>|<span data-ttu-id="95914-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="95914-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95914-126">Relações</span><span class="sxs-lookup"><span data-stu-id="95914-126">Relationships</span></span>
<span data-ttu-id="95914-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95914-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95914-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95914-128">JSON Representation</span></span>
<span data-ttu-id="95914-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95914-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```




