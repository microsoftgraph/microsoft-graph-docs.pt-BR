---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3986bcb6294e2a6da8240e1f1930778fabbeff4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366577"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="1f83c-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="1f83c-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="1f83c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f83c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f83c-105">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1f83c-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="1f83c-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f83c-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f83c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f83c-107">Properties</span></span>
|<span data-ttu-id="1f83c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f83c-108">Property</span></span>|<span data-ttu-id="1f83c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f83c-109">Type</span></span>|<span data-ttu-id="1f83c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f83c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f83c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1f83c-111">displayName</span></span>|<span data-ttu-id="1f83c-112">String</span><span class="sxs-lookup"><span data-stu-id="1f83c-112">String</span></span>|<span data-ttu-id="1f83c-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1f83c-113">Display Name.</span></span> <span data-ttu-id="1f83c-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f83c-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1f83c-115">descrição</span><span class="sxs-lookup"><span data-stu-id="1f83c-115">description</span></span>|<span data-ttu-id="1f83c-116">String</span><span class="sxs-lookup"><span data-stu-id="1f83c-116">String</span></span>|<span data-ttu-id="1f83c-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1f83c-117">Description.</span></span> <span data-ttu-id="1f83c-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f83c-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1f83c-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="1f83c-119">omaUri</span></span>|<span data-ttu-id="1f83c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f83c-120">String</span></span>|<span data-ttu-id="1f83c-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="1f83c-121">OMA.</span></span> <span data-ttu-id="1f83c-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f83c-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1f83c-123">fileName</span><span class="sxs-lookup"><span data-stu-id="1f83c-123">fileName</span></span>|<span data-ttu-id="1f83c-124">String</span><span class="sxs-lookup"><span data-stu-id="1f83c-124">String</span></span>|<span data-ttu-id="1f83c-125">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="1f83c-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="1f83c-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="1f83c-126">\*.crt</span></span> | <span data-ttu-id="1f83c-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="1f83c-127">\*.p7b</span></span> | <span data-ttu-id="1f83c-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="1f83c-128">\*.bin).</span></span>|
|<span data-ttu-id="1f83c-129">value</span><span class="sxs-lookup"><span data-stu-id="1f83c-129">value</span></span>|<span data-ttu-id="1f83c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f83c-130">String</span></span>|<span data-ttu-id="1f83c-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="1f83c-131">Value.</span></span> <span data-ttu-id="1f83c-132">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="1f83c-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f83c-133">Relações</span><span class="sxs-lookup"><span data-stu-id="1f83c-133">Relationships</span></span>
<span data-ttu-id="1f83c-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f83c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f83c-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f83c-135">JSON Representation</span></span>
<span data-ttu-id="1f83c-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f83c-136">Here is a JSON representation of the resource.</span></span>
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




