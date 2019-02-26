---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4d1b1e4c2c02711d341f70bba28067489c3b817
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166805"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="f14ce-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="f14ce-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="f14ce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f14ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f14ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f14ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f14ce-106">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f14ce-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="f14ce-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f14ce-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f14ce-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f14ce-108">Properties</span></span>
|<span data-ttu-id="f14ce-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f14ce-109">Property</span></span>|<span data-ttu-id="f14ce-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f14ce-110">Type</span></span>|<span data-ttu-id="f14ce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f14ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f14ce-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f14ce-112">displayName</span></span>|<span data-ttu-id="f14ce-113">String</span><span class="sxs-lookup"><span data-stu-id="f14ce-113">String</span></span>|<span data-ttu-id="f14ce-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f14ce-114">Display Name.</span></span> <span data-ttu-id="f14ce-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f14ce-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f14ce-116">descrição</span><span class="sxs-lookup"><span data-stu-id="f14ce-116">description</span></span>|<span data-ttu-id="f14ce-117">String</span><span class="sxs-lookup"><span data-stu-id="f14ce-117">String</span></span>|<span data-ttu-id="f14ce-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f14ce-118">Description.</span></span> <span data-ttu-id="f14ce-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f14ce-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f14ce-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f14ce-120">omaUri</span></span>|<span data-ttu-id="f14ce-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f14ce-121">String</span></span>|<span data-ttu-id="f14ce-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="f14ce-122">OMA.</span></span> <span data-ttu-id="f14ce-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f14ce-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f14ce-124">value</span><span class="sxs-lookup"><span data-stu-id="f14ce-124">value</span></span>|<span data-ttu-id="f14ce-125">Single</span><span class="sxs-lookup"><span data-stu-id="f14ce-125">Single</span></span>|<span data-ttu-id="f14ce-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="f14ce-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f14ce-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f14ce-127">Relationships</span></span>
<span data-ttu-id="f14ce-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f14ce-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f14ce-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f14ce-129">JSON Representation</span></span>
<span data-ttu-id="f14ce-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f14ce-130">Here is a JSON representation of the resource.</span></span>
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




