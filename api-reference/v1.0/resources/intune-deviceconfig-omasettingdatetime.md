---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4405f8446ceb76dbdd5b4c9df1407ee14861a3b8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360794"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="72849-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="72849-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="72849-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72849-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72849-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="72849-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="72849-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="72849-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72849-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72849-107">Properties</span></span>
|<span data-ttu-id="72849-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72849-108">Property</span></span>|<span data-ttu-id="72849-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="72849-109">Type</span></span>|<span data-ttu-id="72849-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="72849-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72849-111">displayName</span><span class="sxs-lookup"><span data-stu-id="72849-111">displayName</span></span>|<span data-ttu-id="72849-112">String</span><span class="sxs-lookup"><span data-stu-id="72849-112">String</span></span>|<span data-ttu-id="72849-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="72849-113">Display Name.</span></span> <span data-ttu-id="72849-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="72849-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72849-115">descrição</span><span class="sxs-lookup"><span data-stu-id="72849-115">description</span></span>|<span data-ttu-id="72849-116">String</span><span class="sxs-lookup"><span data-stu-id="72849-116">String</span></span>|<span data-ttu-id="72849-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="72849-117">Description.</span></span> <span data-ttu-id="72849-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="72849-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72849-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="72849-119">omaUri</span></span>|<span data-ttu-id="72849-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72849-120">String</span></span>|<span data-ttu-id="72849-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="72849-121">OMA.</span></span> <span data-ttu-id="72849-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="72849-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="72849-123">value</span><span class="sxs-lookup"><span data-stu-id="72849-123">value</span></span>|<span data-ttu-id="72849-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72849-124">DateTimeOffset</span></span>|<span data-ttu-id="72849-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="72849-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72849-126">Relações</span><span class="sxs-lookup"><span data-stu-id="72849-126">Relationships</span></span>
<span data-ttu-id="72849-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72849-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72849-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72849-128">JSON Representation</span></span>
<span data-ttu-id="72849-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72849-129">Here is a JSON representation of the resource.</span></span>
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




