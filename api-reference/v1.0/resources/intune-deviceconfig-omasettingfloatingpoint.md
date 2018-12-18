---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
ms.openlocfilehash: efed2112f85ee0600fcbe499616a7f3e787beb59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360750"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="e48cf-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="e48cf-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="e48cf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e48cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e48cf-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e48cf-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="e48cf-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e48cf-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e48cf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e48cf-107">Properties</span></span>
|<span data-ttu-id="e48cf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e48cf-108">Property</span></span>|<span data-ttu-id="e48cf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e48cf-109">Type</span></span>|<span data-ttu-id="e48cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e48cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e48cf-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e48cf-111">displayName</span></span>|<span data-ttu-id="e48cf-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e48cf-112">String</span></span>|<span data-ttu-id="e48cf-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e48cf-113">Display Name.</span></span> <span data-ttu-id="e48cf-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e48cf-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e48cf-115">descrição</span><span class="sxs-lookup"><span data-stu-id="e48cf-115">description</span></span>|<span data-ttu-id="e48cf-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e48cf-116">String</span></span>|<span data-ttu-id="e48cf-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e48cf-117">Description.</span></span> <span data-ttu-id="e48cf-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e48cf-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e48cf-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e48cf-119">omaUri</span></span>|<span data-ttu-id="e48cf-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e48cf-120">String</span></span>|<span data-ttu-id="e48cf-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="e48cf-121">OMA.</span></span> <span data-ttu-id="e48cf-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e48cf-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e48cf-123">value</span><span class="sxs-lookup"><span data-stu-id="e48cf-123">value</span></span>|<span data-ttu-id="e48cf-124">Single</span><span class="sxs-lookup"><span data-stu-id="e48cf-124">Single</span></span>|<span data-ttu-id="e48cf-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="e48cf-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48cf-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e48cf-126">Relationships</span></span>
<span data-ttu-id="e48cf-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e48cf-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e48cf-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e48cf-128">JSON Representation</span></span>
<span data-ttu-id="e48cf-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e48cf-129">Here is a JSON representation of the resource.</span></span>
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



