---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
ms.openlocfilehash: 649e3b3d7716122610ac60291ef58cc25e32c4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005149"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="ad871-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="ad871-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="ad871-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad871-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad871-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="ad871-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="ad871-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ad871-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad871-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad871-107">Properties</span></span>
|<span data-ttu-id="ad871-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad871-108">Property</span></span>|<span data-ttu-id="ad871-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad871-109">Type</span></span>|<span data-ttu-id="ad871-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad871-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad871-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ad871-111">displayName</span></span>|<span data-ttu-id="ad871-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad871-112">String</span></span>|<span data-ttu-id="ad871-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ad871-113">Display Name.</span></span> <span data-ttu-id="ad871-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ad871-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ad871-115">descrição</span><span class="sxs-lookup"><span data-stu-id="ad871-115">description</span></span>|<span data-ttu-id="ad871-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad871-116">String</span></span>|<span data-ttu-id="ad871-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="ad871-117">Description.</span></span> <span data-ttu-id="ad871-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ad871-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ad871-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ad871-119">omaUri</span></span>|<span data-ttu-id="ad871-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad871-120">String</span></span>|<span data-ttu-id="ad871-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ad871-121">OMA.</span></span> <span data-ttu-id="ad871-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ad871-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ad871-123">value</span><span class="sxs-lookup"><span data-stu-id="ad871-123">value</span></span>|<span data-ttu-id="ad871-124">Single</span><span class="sxs-lookup"><span data-stu-id="ad871-124">Single</span></span>|<span data-ttu-id="ad871-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="ad871-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad871-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ad871-126">Relationships</span></span>
<span data-ttu-id="ad871-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad871-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad871-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad871-128">JSON Representation</span></span>
<span data-ttu-id="ad871-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad871-129">Here is a JSON representation of the resource.</span></span>
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



