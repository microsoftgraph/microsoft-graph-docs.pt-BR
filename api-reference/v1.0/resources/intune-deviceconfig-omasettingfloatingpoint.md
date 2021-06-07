---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba82e79c16d8aeebd591f55849df74febad0073b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755872"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="126cf-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="126cf-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="126cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="126cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="126cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="126cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="126cf-106">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="126cf-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="126cf-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="126cf-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="126cf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="126cf-108">Properties</span></span>
|<span data-ttu-id="126cf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="126cf-109">Property</span></span>|<span data-ttu-id="126cf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="126cf-110">Type</span></span>|<span data-ttu-id="126cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="126cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="126cf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="126cf-112">displayName</span></span>|<span data-ttu-id="126cf-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="126cf-113">String</span></span>|<span data-ttu-id="126cf-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="126cf-114">Display Name.</span></span> <span data-ttu-id="126cf-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="126cf-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="126cf-116">descrição</span><span class="sxs-lookup"><span data-stu-id="126cf-116">description</span></span>|<span data-ttu-id="126cf-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="126cf-117">String</span></span>|<span data-ttu-id="126cf-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="126cf-118">Description.</span></span> <span data-ttu-id="126cf-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="126cf-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="126cf-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="126cf-120">omaUri</span></span>|<span data-ttu-id="126cf-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="126cf-121">String</span></span>|<span data-ttu-id="126cf-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="126cf-122">OMA.</span></span> <span data-ttu-id="126cf-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="126cf-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="126cf-124">value</span><span class="sxs-lookup"><span data-stu-id="126cf-124">value</span></span>|<span data-ttu-id="126cf-125">Single</span><span class="sxs-lookup"><span data-stu-id="126cf-125">Single</span></span>|<span data-ttu-id="126cf-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="126cf-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="126cf-127">Relações</span><span class="sxs-lookup"><span data-stu-id="126cf-127">Relationships</span></span>
<span data-ttu-id="126cf-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="126cf-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="126cf-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="126cf-129">JSON Representation</span></span>
<span data-ttu-id="126cf-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="126cf-130">Here is a JSON representation of the resource.</span></span>
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
  "value": 4.2
}
```




