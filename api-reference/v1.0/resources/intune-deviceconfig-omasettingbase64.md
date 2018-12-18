---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 6b0835864d3ec8f8364a15ff293a75dfeded3a0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343719"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="472ed-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="472ed-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="472ed-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="472ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="472ed-105">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="472ed-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="472ed-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="472ed-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="472ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="472ed-107">Properties</span></span>
|<span data-ttu-id="472ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="472ed-108">Property</span></span>|<span data-ttu-id="472ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="472ed-109">Type</span></span>|<span data-ttu-id="472ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="472ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472ed-111">displayName</span><span class="sxs-lookup"><span data-stu-id="472ed-111">displayName</span></span>|<span data-ttu-id="472ed-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472ed-112">String</span></span>|<span data-ttu-id="472ed-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="472ed-113">Display Name.</span></span> <span data-ttu-id="472ed-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="472ed-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="472ed-115">descrição</span><span class="sxs-lookup"><span data-stu-id="472ed-115">description</span></span>|<span data-ttu-id="472ed-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472ed-116">String</span></span>|<span data-ttu-id="472ed-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="472ed-117">Description.</span></span> <span data-ttu-id="472ed-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="472ed-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="472ed-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="472ed-119">omaUri</span></span>|<span data-ttu-id="472ed-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472ed-120">String</span></span>|<span data-ttu-id="472ed-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="472ed-121">OMA.</span></span> <span data-ttu-id="472ed-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="472ed-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="472ed-123">fileName</span><span class="sxs-lookup"><span data-stu-id="472ed-123">fileName</span></span>|<span data-ttu-id="472ed-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472ed-124">String</span></span>|<span data-ttu-id="472ed-125">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="472ed-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="472ed-126">CRT</span><span class="sxs-lookup"><span data-stu-id="472ed-126">\*.crt</span></span> | <span data-ttu-id="472ed-127">p7b</span><span class="sxs-lookup"><span data-stu-id="472ed-127">\*.p7b</span></span> | <span data-ttu-id="472ed-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="472ed-128">\*.bin).</span></span>|
|<span data-ttu-id="472ed-129">valor</span><span class="sxs-lookup"><span data-stu-id="472ed-129">value</span></span>|<span data-ttu-id="472ed-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472ed-130">String</span></span>|<span data-ttu-id="472ed-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="472ed-131">Value.</span></span> <span data-ttu-id="472ed-132">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="472ed-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="472ed-133">Relações</span><span class="sxs-lookup"><span data-stu-id="472ed-133">Relationships</span></span>
<span data-ttu-id="472ed-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="472ed-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="472ed-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="472ed-135">JSON Representation</span></span>
<span data-ttu-id="472ed-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="472ed-136">Here is a JSON representation of the resource.</span></span>
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



