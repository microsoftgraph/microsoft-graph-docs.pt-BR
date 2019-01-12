---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34c19caee6bab30dbfe0e82abf1a55f20bb5d3b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932291"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="53b12-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="53b12-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="53b12-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53b12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53b12-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="53b12-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="53b12-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53b12-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53b12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53b12-107">Properties</span></span>
|<span data-ttu-id="53b12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53b12-108">Property</span></span>|<span data-ttu-id="53b12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b12-109">Type</span></span>|<span data-ttu-id="53b12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b12-111">displayName</span><span class="sxs-lookup"><span data-stu-id="53b12-111">displayName</span></span>|<span data-ttu-id="53b12-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b12-112">String</span></span>|<span data-ttu-id="53b12-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="53b12-113">Display Name.</span></span> <span data-ttu-id="53b12-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53b12-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53b12-115">descrição</span><span class="sxs-lookup"><span data-stu-id="53b12-115">description</span></span>|<span data-ttu-id="53b12-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b12-116">String</span></span>|<span data-ttu-id="53b12-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="53b12-117">Description.</span></span> <span data-ttu-id="53b12-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53b12-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53b12-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="53b12-119">omaUri</span></span>|<span data-ttu-id="53b12-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b12-120">String</span></span>|<span data-ttu-id="53b12-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="53b12-121">OMA.</span></span> <span data-ttu-id="53b12-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53b12-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53b12-123">value</span><span class="sxs-lookup"><span data-stu-id="53b12-123">value</span></span>|<span data-ttu-id="53b12-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b12-124">DateTimeOffset</span></span>|<span data-ttu-id="53b12-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="53b12-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53b12-126">Relações</span><span class="sxs-lookup"><span data-stu-id="53b12-126">Relationships</span></span>
<span data-ttu-id="53b12-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53b12-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53b12-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53b12-128">JSON Representation</span></span>
<span data-ttu-id="53b12-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53b12-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



