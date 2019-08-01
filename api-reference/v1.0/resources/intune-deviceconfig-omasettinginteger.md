---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f80f8583907a25646643fdd5770d6bce5adcb4b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028018"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="f81ec-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="f81ec-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="f81ec-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f81ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f81ec-105">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f81ec-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="f81ec-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f81ec-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f81ec-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f81ec-107">Properties</span></span>
|<span data-ttu-id="f81ec-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f81ec-108">Property</span></span>|<span data-ttu-id="f81ec-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f81ec-109">Type</span></span>|<span data-ttu-id="f81ec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f81ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f81ec-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f81ec-111">displayName</span></span>|<span data-ttu-id="f81ec-112">String</span><span class="sxs-lookup"><span data-stu-id="f81ec-112">String</span></span>|<span data-ttu-id="f81ec-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f81ec-113">Display Name.</span></span> <span data-ttu-id="f81ec-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f81ec-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f81ec-115">descrição</span><span class="sxs-lookup"><span data-stu-id="f81ec-115">description</span></span>|<span data-ttu-id="f81ec-116">String</span><span class="sxs-lookup"><span data-stu-id="f81ec-116">String</span></span>|<span data-ttu-id="f81ec-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f81ec-117">Description.</span></span> <span data-ttu-id="f81ec-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f81ec-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f81ec-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f81ec-119">omaUri</span></span>|<span data-ttu-id="f81ec-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81ec-120">String</span></span>|<span data-ttu-id="f81ec-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="f81ec-121">OMA.</span></span> <span data-ttu-id="f81ec-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f81ec-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f81ec-123">valor</span><span class="sxs-lookup"><span data-stu-id="f81ec-123">value</span></span>|<span data-ttu-id="f81ec-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f81ec-124">Int32</span></span>|<span data-ttu-id="f81ec-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="f81ec-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f81ec-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f81ec-126">Relationships</span></span>
<span data-ttu-id="f81ec-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f81ec-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f81ec-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f81ec-128">JSON Representation</span></span>
<span data-ttu-id="f81ec-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f81ec-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



