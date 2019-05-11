---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8affdb1f073831df54837420b54f9a0ea19ad956
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951040"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="6f9de-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="6f9de-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="6f9de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f9de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f9de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f9de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f9de-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="6f9de-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="6f9de-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f9de-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f9de-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f9de-108">Properties</span></span>
|<span data-ttu-id="6f9de-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f9de-109">Property</span></span>|<span data-ttu-id="6f9de-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f9de-110">Type</span></span>|<span data-ttu-id="6f9de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f9de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9de-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6f9de-112">displayName</span></span>|<span data-ttu-id="6f9de-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f9de-113">String</span></span>|<span data-ttu-id="6f9de-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6f9de-114">Display Name.</span></span> <span data-ttu-id="6f9de-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f9de-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6f9de-116">description</span><span class="sxs-lookup"><span data-stu-id="6f9de-116">description</span></span>|<span data-ttu-id="6f9de-117">String</span><span class="sxs-lookup"><span data-stu-id="6f9de-117">String</span></span>|<span data-ttu-id="6f9de-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="6f9de-118">Description.</span></span> <span data-ttu-id="6f9de-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f9de-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6f9de-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="6f9de-120">omaUri</span></span>|<span data-ttu-id="6f9de-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f9de-121">String</span></span>|<span data-ttu-id="6f9de-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="6f9de-122">OMA.</span></span> <span data-ttu-id="6f9de-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6f9de-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6f9de-124">fileName</span><span class="sxs-lookup"><span data-stu-id="6f9de-124">fileName</span></span>|<span data-ttu-id="6f9de-125">String</span><span class="sxs-lookup"><span data-stu-id="6f9de-125">String</span></span>|<span data-ttu-id="6f9de-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="6f9de-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="6f9de-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="6f9de-127">\*.crt</span></span> | <span data-ttu-id="6f9de-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="6f9de-128">\*.p7b</span></span> | <span data-ttu-id="6f9de-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="6f9de-129">\*.bin).</span></span>|
|<span data-ttu-id="6f9de-130">value</span><span class="sxs-lookup"><span data-stu-id="6f9de-130">value</span></span>|<span data-ttu-id="6f9de-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f9de-131">String</span></span>|<span data-ttu-id="6f9de-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="6f9de-132">Value.</span></span> <span data-ttu-id="6f9de-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="6f9de-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f9de-134">Relações</span><span class="sxs-lookup"><span data-stu-id="6f9de-134">Relationships</span></span>
<span data-ttu-id="6f9de-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f9de-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f9de-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f9de-136">JSON Representation</span></span>
<span data-ttu-id="6f9de-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f9de-137">Here is a JSON representation of the resource.</span></span>
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




