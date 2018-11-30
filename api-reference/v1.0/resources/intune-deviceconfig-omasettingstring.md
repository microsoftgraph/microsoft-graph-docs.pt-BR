---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
ms.openlocfilehash: 543b993ee557c47e415a2f19f9791b0685c818e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004414"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="a321e-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="a321e-103">omaSettingString resource type</span></span>

> <span data-ttu-id="a321e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a321e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a321e-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a321e-105">OMA Settings String definition.</span></span>

<span data-ttu-id="a321e-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a321e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a321e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a321e-107">Properties</span></span>
|<span data-ttu-id="a321e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a321e-108">Property</span></span>|<span data-ttu-id="a321e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a321e-109">Type</span></span>|<span data-ttu-id="a321e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a321e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a321e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a321e-111">displayName</span></span>|<span data-ttu-id="a321e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a321e-112">String</span></span>|<span data-ttu-id="a321e-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a321e-113">Display Name.</span></span> <span data-ttu-id="a321e-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a321e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a321e-115">descrição</span><span class="sxs-lookup"><span data-stu-id="a321e-115">description</span></span>|<span data-ttu-id="a321e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a321e-116">String</span></span>|<span data-ttu-id="a321e-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a321e-117">Description.</span></span> <span data-ttu-id="a321e-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a321e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a321e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a321e-119">omaUri</span></span>|<span data-ttu-id="a321e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a321e-120">String</span></span>|<span data-ttu-id="a321e-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="a321e-121">OMA.</span></span> <span data-ttu-id="a321e-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a321e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a321e-123">valor</span><span class="sxs-lookup"><span data-stu-id="a321e-123">value</span></span>|<span data-ttu-id="a321e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a321e-124">String</span></span>|<span data-ttu-id="a321e-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="a321e-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a321e-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a321e-126">Relationships</span></span>
<span data-ttu-id="a321e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a321e-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a321e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a321e-128">JSON Representation</span></span>
<span data-ttu-id="a321e-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a321e-129">Here is a JSON representation of the resource.</span></span>
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



