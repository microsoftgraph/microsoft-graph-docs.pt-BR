---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e95f17d0b9e4a8347c71042244100c96590a527
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788475"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c8326-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="c8326-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="c8326-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8326-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8326-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8326-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8326-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="c8326-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="c8326-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c8326-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8326-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8326-108">Properties</span></span>
|<span data-ttu-id="c8326-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8326-109">Property</span></span>|<span data-ttu-id="c8326-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8326-110">Type</span></span>|<span data-ttu-id="c8326-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8326-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8326-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c8326-112">displayName</span></span>|<span data-ttu-id="c8326-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8326-113">String</span></span>|<span data-ttu-id="c8326-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="c8326-114">Display Name.</span></span> <span data-ttu-id="c8326-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c8326-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c8326-116">description</span><span class="sxs-lookup"><span data-stu-id="c8326-116">description</span></span>|<span data-ttu-id="c8326-117">String</span><span class="sxs-lookup"><span data-stu-id="c8326-117">String</span></span>|<span data-ttu-id="c8326-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="c8326-118">Description.</span></span> <span data-ttu-id="c8326-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c8326-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c8326-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="c8326-120">omaUri</span></span>|<span data-ttu-id="c8326-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8326-121">String</span></span>|<span data-ttu-id="c8326-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="c8326-122">OMA.</span></span> <span data-ttu-id="c8326-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c8326-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c8326-124">fileName</span><span class="sxs-lookup"><span data-stu-id="c8326-124">fileName</span></span>|<span data-ttu-id="c8326-125">String</span><span class="sxs-lookup"><span data-stu-id="c8326-125">String</span></span>|<span data-ttu-id="c8326-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="c8326-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c8326-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="c8326-127">\*.crt</span></span> | <span data-ttu-id="c8326-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="c8326-128">\*.p7b</span></span> | <span data-ttu-id="c8326-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="c8326-129">\*.bin).</span></span>|
|<span data-ttu-id="c8326-130">value</span><span class="sxs-lookup"><span data-stu-id="c8326-130">value</span></span>|<span data-ttu-id="c8326-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8326-131">String</span></span>|<span data-ttu-id="c8326-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="c8326-132">Value.</span></span> <span data-ttu-id="c8326-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="c8326-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8326-134">Relações</span><span class="sxs-lookup"><span data-stu-id="c8326-134">Relationships</span></span>
<span data-ttu-id="c8326-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8326-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8326-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8326-136">JSON Representation</span></span>
<span data-ttu-id="c8326-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8326-137">Here is a JSON representation of the resource.</span></span>
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



