---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33488e3b6500056c0f183d5e219e5f5ec489c178
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787068"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="618bc-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="618bc-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="618bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="618bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="618bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="618bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="618bc-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="618bc-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="618bc-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="618bc-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="618bc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="618bc-108">Properties</span></span>
|<span data-ttu-id="618bc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="618bc-109">Property</span></span>|<span data-ttu-id="618bc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="618bc-110">Type</span></span>|<span data-ttu-id="618bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="618bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="618bc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="618bc-112">displayName</span></span>|<span data-ttu-id="618bc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="618bc-113">String</span></span>|<span data-ttu-id="618bc-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="618bc-114">Display Name.</span></span> <span data-ttu-id="618bc-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="618bc-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="618bc-116">description</span><span class="sxs-lookup"><span data-stu-id="618bc-116">description</span></span>|<span data-ttu-id="618bc-117">String</span><span class="sxs-lookup"><span data-stu-id="618bc-117">String</span></span>|<span data-ttu-id="618bc-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="618bc-118">Description.</span></span> <span data-ttu-id="618bc-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="618bc-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="618bc-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="618bc-120">omaUri</span></span>|<span data-ttu-id="618bc-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="618bc-121">String</span></span>|<span data-ttu-id="618bc-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="618bc-122">OMA.</span></span> <span data-ttu-id="618bc-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="618bc-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="618bc-124">fileName</span><span class="sxs-lookup"><span data-stu-id="618bc-124">fileName</span></span>|<span data-ttu-id="618bc-125">String</span><span class="sxs-lookup"><span data-stu-id="618bc-125">String</span></span>|<span data-ttu-id="618bc-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="618bc-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="618bc-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="618bc-127">\*.crt</span></span> | <span data-ttu-id="618bc-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="618bc-128">\*.p7b</span></span> | <span data-ttu-id="618bc-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="618bc-129">\*.bin).</span></span>|
|<span data-ttu-id="618bc-130">value</span><span class="sxs-lookup"><span data-stu-id="618bc-130">value</span></span>|<span data-ttu-id="618bc-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="618bc-131">String</span></span>|<span data-ttu-id="618bc-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="618bc-132">Value.</span></span> <span data-ttu-id="618bc-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="618bc-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="618bc-134">Relações</span><span class="sxs-lookup"><span data-stu-id="618bc-134">Relationships</span></span>
<span data-ttu-id="618bc-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="618bc-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="618bc-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="618bc-136">JSON Representation</span></span>
<span data-ttu-id="618bc-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="618bc-137">Here is a JSON representation of the resource.</span></span>
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





