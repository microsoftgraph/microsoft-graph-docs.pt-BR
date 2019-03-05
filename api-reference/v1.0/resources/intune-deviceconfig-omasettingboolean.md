---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256389"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="28fc3-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="28fc3-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="28fc3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28fc3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28fc3-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="28fc3-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="28fc3-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="28fc3-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28fc3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28fc3-107">Properties</span></span>
|<span data-ttu-id="28fc3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28fc3-108">Property</span></span>|<span data-ttu-id="28fc3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28fc3-109">Type</span></span>|<span data-ttu-id="28fc3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28fc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28fc3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="28fc3-111">displayName</span></span>|<span data-ttu-id="28fc3-112">String</span><span class="sxs-lookup"><span data-stu-id="28fc3-112">String</span></span>|<span data-ttu-id="28fc3-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="28fc3-113">Display Name.</span></span> <span data-ttu-id="28fc3-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="28fc3-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="28fc3-115">descrição</span><span class="sxs-lookup"><span data-stu-id="28fc3-115">description</span></span>|<span data-ttu-id="28fc3-116">String</span><span class="sxs-lookup"><span data-stu-id="28fc3-116">String</span></span>|<span data-ttu-id="28fc3-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="28fc3-117">Description.</span></span> <span data-ttu-id="28fc3-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="28fc3-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="28fc3-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="28fc3-119">omaUri</span></span>|<span data-ttu-id="28fc3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28fc3-120">String</span></span>|<span data-ttu-id="28fc3-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="28fc3-121">OMA.</span></span> <span data-ttu-id="28fc3-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="28fc3-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="28fc3-123">valor</span><span class="sxs-lookup"><span data-stu-id="28fc3-123">value</span></span>|<span data-ttu-id="28fc3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="28fc3-124">Boolean</span></span>|<span data-ttu-id="28fc3-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="28fc3-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28fc3-126">Relações</span><span class="sxs-lookup"><span data-stu-id="28fc3-126">Relationships</span></span>
<span data-ttu-id="28fc3-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28fc3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28fc3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28fc3-128">JSON Representation</span></span>
<span data-ttu-id="28fc3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28fc3-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



