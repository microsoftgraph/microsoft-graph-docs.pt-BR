---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a36d30cb62862b469d7b32d742275d399ed36db0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888127"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="a4450-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="a4450-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="a4450-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a4450-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4450-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a4450-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="a4450-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a4450-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4450-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4450-107">Properties</span></span>
|<span data-ttu-id="a4450-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4450-108">Property</span></span>|<span data-ttu-id="a4450-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4450-109">Type</span></span>|<span data-ttu-id="a4450-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4450-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4450-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a4450-111">displayName</span></span>|<span data-ttu-id="a4450-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4450-112">String</span></span>|<span data-ttu-id="a4450-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a4450-113">Display Name.</span></span> <span data-ttu-id="a4450-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a4450-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a4450-115">descrição</span><span class="sxs-lookup"><span data-stu-id="a4450-115">description</span></span>|<span data-ttu-id="a4450-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4450-116">String</span></span>|<span data-ttu-id="a4450-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a4450-117">Description.</span></span> <span data-ttu-id="a4450-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a4450-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a4450-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a4450-119">omaUri</span></span>|<span data-ttu-id="a4450-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4450-120">String</span></span>|<span data-ttu-id="a4450-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="a4450-121">OMA.</span></span> <span data-ttu-id="a4450-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a4450-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a4450-123">value</span><span class="sxs-lookup"><span data-stu-id="a4450-123">value</span></span>|<span data-ttu-id="a4450-124">Single</span><span class="sxs-lookup"><span data-stu-id="a4450-124">Single</span></span>|<span data-ttu-id="a4450-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="a4450-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4450-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a4450-126">Relationships</span></span>
<span data-ttu-id="a4450-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4450-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4450-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4450-128">JSON Representation</span></span>
<span data-ttu-id="a4450-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4450-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



