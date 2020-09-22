---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff036a8d3bac70193f9653f42fb5380a8d1f0fbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084902"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="ee00a-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="ee00a-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="ee00a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee00a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee00a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee00a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee00a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee00a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee00a-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="ee00a-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="ee00a-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee00a-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee00a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee00a-109">Properties</span></span>
|<span data-ttu-id="ee00a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee00a-110">Property</span></span>|<span data-ttu-id="ee00a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee00a-111">Type</span></span>|<span data-ttu-id="ee00a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee00a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee00a-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ee00a-113">displayName</span></span>|<span data-ttu-id="ee00a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee00a-114">String</span></span>|<span data-ttu-id="ee00a-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ee00a-115">Display Name.</span></span> <span data-ttu-id="ee00a-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee00a-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee00a-117">description</span><span class="sxs-lookup"><span data-stu-id="ee00a-117">description</span></span>|<span data-ttu-id="ee00a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee00a-118">String</span></span>|<span data-ttu-id="ee00a-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="ee00a-119">Description.</span></span> <span data-ttu-id="ee00a-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee00a-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee00a-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ee00a-121">omaUri</span></span>|<span data-ttu-id="ee00a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee00a-122">String</span></span>|<span data-ttu-id="ee00a-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="ee00a-123">OMA.</span></span> <span data-ttu-id="ee00a-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee00a-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee00a-125">fileName</span><span class="sxs-lookup"><span data-stu-id="ee00a-125">fileName</span></span>|<span data-ttu-id="ee00a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee00a-126">String</span></span>|<span data-ttu-id="ee00a-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="ee00a-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="ee00a-128">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="ee00a-128">\*.crt</span></span> | <span data-ttu-id="ee00a-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="ee00a-129">\*.p7b</span></span> | <span data-ttu-id="ee00a-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="ee00a-130">\*.bin).</span></span>|
|<span data-ttu-id="ee00a-131">value</span><span class="sxs-lookup"><span data-stu-id="ee00a-131">value</span></span>|<span data-ttu-id="ee00a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee00a-132">String</span></span>|<span data-ttu-id="ee00a-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="ee00a-133">Value.</span></span> <span data-ttu-id="ee00a-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="ee00a-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee00a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="ee00a-135">Relationships</span></span>
<span data-ttu-id="ee00a-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee00a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee00a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee00a-137">JSON Representation</span></span>
<span data-ttu-id="ee00a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee00a-138">Here is a JSON representation of the resource.</span></span>
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






