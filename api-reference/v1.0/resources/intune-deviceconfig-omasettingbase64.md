---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258587"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="3ff44-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="3ff44-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="3ff44-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ff44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff44-105">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="3ff44-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="3ff44-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ff44-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ff44-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ff44-107">Properties</span></span>
|<span data-ttu-id="3ff44-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ff44-108">Property</span></span>|<span data-ttu-id="3ff44-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ff44-109">Type</span></span>|<span data-ttu-id="3ff44-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff44-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff44-111">displayName</span></span>|<span data-ttu-id="3ff44-112">String</span><span class="sxs-lookup"><span data-stu-id="3ff44-112">String</span></span>|<span data-ttu-id="3ff44-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3ff44-113">Display Name.</span></span> <span data-ttu-id="3ff44-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ff44-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ff44-115">descrição</span><span class="sxs-lookup"><span data-stu-id="3ff44-115">description</span></span>|<span data-ttu-id="3ff44-116">String</span><span class="sxs-lookup"><span data-stu-id="3ff44-116">String</span></span>|<span data-ttu-id="3ff44-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3ff44-117">Description.</span></span> <span data-ttu-id="3ff44-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ff44-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ff44-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="3ff44-119">omaUri</span></span>|<span data-ttu-id="3ff44-120">String</span><span class="sxs-lookup"><span data-stu-id="3ff44-120">String</span></span>|<span data-ttu-id="3ff44-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="3ff44-121">OMA.</span></span> <span data-ttu-id="3ff44-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ff44-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ff44-123">fileName</span><span class="sxs-lookup"><span data-stu-id="3ff44-123">fileName</span></span>|<span data-ttu-id="3ff44-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ff44-124">String</span></span>|<span data-ttu-id="3ff44-125">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="3ff44-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="3ff44-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="3ff44-126">\*.crt</span></span> | <span data-ttu-id="3ff44-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="3ff44-127">\*.p7b</span></span> | <span data-ttu-id="3ff44-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="3ff44-128">\*.bin).</span></span>|
|<span data-ttu-id="3ff44-129">valor</span><span class="sxs-lookup"><span data-stu-id="3ff44-129">value</span></span>|<span data-ttu-id="3ff44-130">String</span><span class="sxs-lookup"><span data-stu-id="3ff44-130">String</span></span>|<span data-ttu-id="3ff44-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="3ff44-131">Value.</span></span> <span data-ttu-id="3ff44-132">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="3ff44-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ff44-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3ff44-133">Relationships</span></span>
<span data-ttu-id="3ff44-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ff44-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ff44-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ff44-135">JSON Representation</span></span>
<span data-ttu-id="3ff44-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ff44-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



