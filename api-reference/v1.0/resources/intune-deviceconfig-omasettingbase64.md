---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72c7bdd9eda67d9bdebc2452ad778d4ad653d7df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079274"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e85a3-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="e85a3-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="e85a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e85a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e85a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e85a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e85a3-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e85a3-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e85a3-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e85a3-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e85a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e85a3-108">Properties</span></span>
|<span data-ttu-id="e85a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e85a3-109">Property</span></span>|<span data-ttu-id="e85a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e85a3-110">Type</span></span>|<span data-ttu-id="e85a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e85a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e85a3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e85a3-112">displayName</span></span>|<span data-ttu-id="e85a3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e85a3-113">String</span></span>|<span data-ttu-id="e85a3-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e85a3-114">Display Name.</span></span> <span data-ttu-id="e85a3-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e85a3-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e85a3-116">description</span><span class="sxs-lookup"><span data-stu-id="e85a3-116">description</span></span>|<span data-ttu-id="e85a3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e85a3-117">String</span></span>|<span data-ttu-id="e85a3-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e85a3-118">Description.</span></span> <span data-ttu-id="e85a3-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e85a3-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e85a3-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="e85a3-120">omaUri</span></span>|<span data-ttu-id="e85a3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e85a3-121">String</span></span>|<span data-ttu-id="e85a3-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="e85a3-122">OMA.</span></span> <span data-ttu-id="e85a3-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e85a3-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e85a3-124">fileName</span><span class="sxs-lookup"><span data-stu-id="e85a3-124">fileName</span></span>|<span data-ttu-id="e85a3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e85a3-125">String</span></span>|<span data-ttu-id="e85a3-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="e85a3-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e85a3-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="e85a3-127">\*.crt</span></span> | <span data-ttu-id="e85a3-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="e85a3-128">\*.p7b</span></span> | <span data-ttu-id="e85a3-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="e85a3-129">\*.bin).</span></span>|
|<span data-ttu-id="e85a3-130">value</span><span class="sxs-lookup"><span data-stu-id="e85a3-130">value</span></span>|<span data-ttu-id="e85a3-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e85a3-131">String</span></span>|<span data-ttu-id="e85a3-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="e85a3-132">Value.</span></span> <span data-ttu-id="e85a3-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="e85a3-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e85a3-134">Relações</span><span class="sxs-lookup"><span data-stu-id="e85a3-134">Relationships</span></span>
<span data-ttu-id="e85a3-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e85a3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e85a3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e85a3-136">JSON Representation</span></span>
<span data-ttu-id="e85a3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e85a3-137">Here is a JSON representation of the resource.</span></span>
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









