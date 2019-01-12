---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46398e43f2a7ea224a07b1637deca2c3a6ed067
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987528"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="71a2d-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="71a2d-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="71a2d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71a2d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71a2d-105">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="71a2d-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="71a2d-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="71a2d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71a2d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71a2d-107">Properties</span></span>
|<span data-ttu-id="71a2d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71a2d-108">Property</span></span>|<span data-ttu-id="71a2d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="71a2d-109">Type</span></span>|<span data-ttu-id="71a2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71a2d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="71a2d-111">displayName</span></span>|<span data-ttu-id="71a2d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a2d-112">String</span></span>|<span data-ttu-id="71a2d-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="71a2d-113">Display Name.</span></span> <span data-ttu-id="71a2d-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="71a2d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="71a2d-115">descrição</span><span class="sxs-lookup"><span data-stu-id="71a2d-115">description</span></span>|<span data-ttu-id="71a2d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a2d-116">String</span></span>|<span data-ttu-id="71a2d-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="71a2d-117">Description.</span></span> <span data-ttu-id="71a2d-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="71a2d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="71a2d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="71a2d-119">omaUri</span></span>|<span data-ttu-id="71a2d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a2d-120">String</span></span>|<span data-ttu-id="71a2d-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="71a2d-121">OMA.</span></span> <span data-ttu-id="71a2d-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="71a2d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="71a2d-123">valor</span><span class="sxs-lookup"><span data-stu-id="71a2d-123">value</span></span>|<span data-ttu-id="71a2d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="71a2d-124">Int32</span></span>|<span data-ttu-id="71a2d-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="71a2d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71a2d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="71a2d-126">Relationships</span></span>
<span data-ttu-id="71a2d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71a2d-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71a2d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71a2d-128">JSON Representation</span></span>
<span data-ttu-id="71a2d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71a2d-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



