---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5fd4df9b5deb49745d337632cfe103fdaad0581
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011425"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e3996-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="e3996-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="e3996-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3996-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3996-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3996-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3996-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e3996-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e3996-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3996-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3996-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3996-108">Properties</span></span>
|<span data-ttu-id="e3996-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3996-109">Property</span></span>|<span data-ttu-id="e3996-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3996-110">Type</span></span>|<span data-ttu-id="e3996-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3996-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3996-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e3996-112">displayName</span></span>|<span data-ttu-id="e3996-113">String</span><span class="sxs-lookup"><span data-stu-id="e3996-113">String</span></span>|<span data-ttu-id="e3996-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e3996-114">Display Name.</span></span> <span data-ttu-id="e3996-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3996-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3996-116">descrição</span><span class="sxs-lookup"><span data-stu-id="e3996-116">description</span></span>|<span data-ttu-id="e3996-117">String</span><span class="sxs-lookup"><span data-stu-id="e3996-117">String</span></span>|<span data-ttu-id="e3996-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e3996-118">Description.</span></span> <span data-ttu-id="e3996-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3996-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3996-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="e3996-120">omaUri</span></span>|<span data-ttu-id="e3996-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3996-121">String</span></span>|<span data-ttu-id="e3996-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="e3996-122">OMA.</span></span> <span data-ttu-id="e3996-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3996-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3996-124">fileName</span><span class="sxs-lookup"><span data-stu-id="e3996-124">fileName</span></span>|<span data-ttu-id="e3996-125">String</span><span class="sxs-lookup"><span data-stu-id="e3996-125">String</span></span>|<span data-ttu-id="e3996-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="e3996-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e3996-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="e3996-127">\*.crt</span></span> | <span data-ttu-id="e3996-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="e3996-128">\*.p7b</span></span> | <span data-ttu-id="e3996-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="e3996-129">\*.bin).</span></span>|
|<span data-ttu-id="e3996-130">value</span><span class="sxs-lookup"><span data-stu-id="e3996-130">value</span></span>|<span data-ttu-id="e3996-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3996-131">String</span></span>|<span data-ttu-id="e3996-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="e3996-132">Value.</span></span> <span data-ttu-id="e3996-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="e3996-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3996-134">Relações</span><span class="sxs-lookup"><span data-stu-id="e3996-134">Relationships</span></span>
<span data-ttu-id="e3996-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3996-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3996-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3996-136">JSON Representation</span></span>
<span data-ttu-id="e3996-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3996-137">Here is a JSON representation of the resource.</span></span>
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





