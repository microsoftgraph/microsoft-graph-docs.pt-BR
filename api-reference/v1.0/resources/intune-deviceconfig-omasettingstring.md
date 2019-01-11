---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 890d636afb29fbfb188e9c1b514eecc6360001b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841346"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="74867-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="74867-103">omaSettingString resource type</span></span>

> <span data-ttu-id="74867-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74867-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74867-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="74867-105">OMA Settings String definition.</span></span>

<span data-ttu-id="74867-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74867-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74867-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74867-107">Properties</span></span>
|<span data-ttu-id="74867-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74867-108">Property</span></span>|<span data-ttu-id="74867-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="74867-109">Type</span></span>|<span data-ttu-id="74867-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="74867-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74867-111">displayName</span><span class="sxs-lookup"><span data-stu-id="74867-111">displayName</span></span>|<span data-ttu-id="74867-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74867-112">String</span></span>|<span data-ttu-id="74867-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="74867-113">Display Name.</span></span> <span data-ttu-id="74867-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74867-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74867-115">descrição</span><span class="sxs-lookup"><span data-stu-id="74867-115">description</span></span>|<span data-ttu-id="74867-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74867-116">String</span></span>|<span data-ttu-id="74867-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="74867-117">Description.</span></span> <span data-ttu-id="74867-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74867-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74867-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="74867-119">omaUri</span></span>|<span data-ttu-id="74867-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74867-120">String</span></span>|<span data-ttu-id="74867-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="74867-121">OMA.</span></span> <span data-ttu-id="74867-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74867-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74867-123">valor</span><span class="sxs-lookup"><span data-stu-id="74867-123">value</span></span>|<span data-ttu-id="74867-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74867-124">String</span></span>|<span data-ttu-id="74867-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="74867-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74867-126">Relações</span><span class="sxs-lookup"><span data-stu-id="74867-126">Relationships</span></span>
<span data-ttu-id="74867-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74867-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74867-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74867-128">JSON Representation</span></span>
<span data-ttu-id="74867-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74867-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



