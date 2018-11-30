---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
ms.openlocfilehash: 891c13a4cfcc8c0cf378cb5c7f9c6449bd876b7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006046"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="32295-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="32295-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="32295-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32295-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32295-105">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="32295-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="32295-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="32295-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32295-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32295-107">Properties</span></span>
|<span data-ttu-id="32295-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32295-108">Property</span></span>|<span data-ttu-id="32295-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="32295-109">Type</span></span>|<span data-ttu-id="32295-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32295-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32295-111">displayName</span><span class="sxs-lookup"><span data-stu-id="32295-111">displayName</span></span>|<span data-ttu-id="32295-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32295-112">String</span></span>|<span data-ttu-id="32295-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="32295-113">Display Name.</span></span> <span data-ttu-id="32295-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="32295-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="32295-115">descrição</span><span class="sxs-lookup"><span data-stu-id="32295-115">description</span></span>|<span data-ttu-id="32295-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32295-116">String</span></span>|<span data-ttu-id="32295-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="32295-117">Description.</span></span> <span data-ttu-id="32295-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="32295-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="32295-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="32295-119">omaUri</span></span>|<span data-ttu-id="32295-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32295-120">String</span></span>|<span data-ttu-id="32295-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="32295-121">OMA.</span></span> <span data-ttu-id="32295-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="32295-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="32295-123">fileName</span><span class="sxs-lookup"><span data-stu-id="32295-123">fileName</span></span>|<span data-ttu-id="32295-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32295-124">String</span></span>|<span data-ttu-id="32295-125">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="32295-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="32295-126">CRT</span><span class="sxs-lookup"><span data-stu-id="32295-126">\*.crt</span></span> | <span data-ttu-id="32295-127">p7b</span><span class="sxs-lookup"><span data-stu-id="32295-127">\*.p7b</span></span> | <span data-ttu-id="32295-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="32295-128">\*.bin).</span></span>|
|<span data-ttu-id="32295-129">valor</span><span class="sxs-lookup"><span data-stu-id="32295-129">value</span></span>|<span data-ttu-id="32295-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32295-130">String</span></span>|<span data-ttu-id="32295-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="32295-131">Value.</span></span> <span data-ttu-id="32295-132">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="32295-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="32295-133">Relações</span><span class="sxs-lookup"><span data-stu-id="32295-133">Relationships</span></span>
<span data-ttu-id="32295-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32295-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32295-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32295-135">JSON Representation</span></span>
<span data-ttu-id="32295-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32295-136">Here is a JSON representation of the resource.</span></span>
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



