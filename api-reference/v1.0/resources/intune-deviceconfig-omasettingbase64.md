---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cfbe888eb5bbe10fc974a91769246d025d284c39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751388"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="f5fd0-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="f5fd0-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="f5fd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5fd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5fd0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5fd0-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="f5fd0-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5fd0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5fd0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5fd0-108">Properties</span></span>
|<span data-ttu-id="f5fd0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5fd0-109">Property</span></span>|<span data-ttu-id="f5fd0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5fd0-110">Type</span></span>|<span data-ttu-id="f5fd0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5fd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5fd0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f5fd0-112">displayName</span></span>|<span data-ttu-id="f5fd0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fd0-113">String</span></span>|<span data-ttu-id="f5fd0-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-114">Display Name.</span></span> <span data-ttu-id="f5fd0-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5fd0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5fd0-116">descrição</span><span class="sxs-lookup"><span data-stu-id="f5fd0-116">description</span></span>|<span data-ttu-id="f5fd0-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fd0-117">String</span></span>|<span data-ttu-id="f5fd0-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-118">Description.</span></span> <span data-ttu-id="f5fd0-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5fd0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5fd0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f5fd0-120">omaUri</span></span>|<span data-ttu-id="f5fd0-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fd0-121">String</span></span>|<span data-ttu-id="f5fd0-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-122">OMA.</span></span> <span data-ttu-id="f5fd0-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f5fd0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f5fd0-124">fileName</span><span class="sxs-lookup"><span data-stu-id="f5fd0-124">fileName</span></span>|<span data-ttu-id="f5fd0-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fd0-125">String</span></span>|<span data-ttu-id="f5fd0-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="f5fd0-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="f5fd0-127">\*.crt</span><span class="sxs-lookup"><span data-stu-id="f5fd0-127">\*.crt</span></span> | <span data-ttu-id="f5fd0-128">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="f5fd0-128">\*.p7b</span></span> | <span data-ttu-id="f5fd0-129">\*.bin).</span><span class="sxs-lookup"><span data-stu-id="f5fd0-129">\*.bin).</span></span>|
|<span data-ttu-id="f5fd0-130">value</span><span class="sxs-lookup"><span data-stu-id="f5fd0-130">value</span></span>|<span data-ttu-id="f5fd0-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fd0-131">String</span></span>|<span data-ttu-id="f5fd0-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-132">Value.</span></span> <span data-ttu-id="f5fd0-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="f5fd0-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5fd0-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f5fd0-134">Relationships</span></span>
<span data-ttu-id="f5fd0-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f5fd0-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5fd0-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5fd0-136">JSON Representation</span></span>
<span data-ttu-id="f5fd0-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5fd0-137">Here is a JSON representation of the resource.</span></span>
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




