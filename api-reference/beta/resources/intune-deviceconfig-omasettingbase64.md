---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f5089c40e2c79d0a3a2e9a920de10d8e5eb4bc1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402002"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="b0190-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="b0190-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="b0190-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0190-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0190-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0190-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0190-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0190-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b0190-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="b0190-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b0190-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0190-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0190-109">Properties</span></span>
|<span data-ttu-id="b0190-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0190-110">Property</span></span>|<span data-ttu-id="b0190-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0190-111">Type</span></span>|<span data-ttu-id="b0190-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0190-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0190-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b0190-113">displayName</span></span>|<span data-ttu-id="b0190-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0190-114">String</span></span>|<span data-ttu-id="b0190-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b0190-115">Display Name.</span></span> <span data-ttu-id="b0190-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b0190-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b0190-117">description</span><span class="sxs-lookup"><span data-stu-id="b0190-117">description</span></span>|<span data-ttu-id="b0190-118">String</span><span class="sxs-lookup"><span data-stu-id="b0190-118">String</span></span>|<span data-ttu-id="b0190-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b0190-119">Description.</span></span> <span data-ttu-id="b0190-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b0190-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b0190-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b0190-121">omaUri</span></span>|<span data-ttu-id="b0190-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0190-122">String</span></span>|<span data-ttu-id="b0190-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="b0190-123">OMA.</span></span> <span data-ttu-id="b0190-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b0190-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b0190-125">fileName</span><span class="sxs-lookup"><span data-stu-id="b0190-125">fileName</span></span>|<span data-ttu-id="b0190-126">String</span><span class="sxs-lookup"><span data-stu-id="b0190-126">String</span></span>|<span data-ttu-id="b0190-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="b0190-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="b0190-128">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="b0190-128">\*.crt</span></span> | <span data-ttu-id="b0190-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="b0190-129">\*.p7b</span></span> | <span data-ttu-id="b0190-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="b0190-130">\*.bin).</span></span>|
|<span data-ttu-id="b0190-131">value</span><span class="sxs-lookup"><span data-stu-id="b0190-131">value</span></span>|<span data-ttu-id="b0190-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0190-132">String</span></span>|<span data-ttu-id="b0190-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="b0190-133">Value.</span></span> <span data-ttu-id="b0190-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="b0190-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0190-135">Relações</span><span class="sxs-lookup"><span data-stu-id="b0190-135">Relationships</span></span>
<span data-ttu-id="b0190-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0190-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0190-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0190-137">JSON Representation</span></span>
<span data-ttu-id="b0190-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0190-138">Here is a JSON representation of the resource.</span></span>
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



