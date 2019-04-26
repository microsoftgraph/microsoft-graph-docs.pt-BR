---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568994"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="5474d-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="5474d-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="5474d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5474d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5474d-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="5474d-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="5474d-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5474d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5474d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5474d-107">Properties</span></span>
|<span data-ttu-id="5474d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5474d-108">Property</span></span>|<span data-ttu-id="5474d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5474d-109">Type</span></span>|<span data-ttu-id="5474d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5474d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5474d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5474d-111">displayName</span></span>|<span data-ttu-id="5474d-112">String</span><span class="sxs-lookup"><span data-stu-id="5474d-112">String</span></span>|<span data-ttu-id="5474d-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="5474d-113">Display Name.</span></span> <span data-ttu-id="5474d-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5474d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5474d-115">description</span><span class="sxs-lookup"><span data-stu-id="5474d-115">description</span></span>|<span data-ttu-id="5474d-116">String</span><span class="sxs-lookup"><span data-stu-id="5474d-116">String</span></span>|<span data-ttu-id="5474d-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="5474d-117">Description.</span></span> <span data-ttu-id="5474d-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5474d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5474d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="5474d-119">omaUri</span></span>|<span data-ttu-id="5474d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5474d-120">String</span></span>|<span data-ttu-id="5474d-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="5474d-121">OMA.</span></span> <span data-ttu-id="5474d-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5474d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5474d-123">value</span><span class="sxs-lookup"><span data-stu-id="5474d-123">value</span></span>|<span data-ttu-id="5474d-124">Single</span><span class="sxs-lookup"><span data-stu-id="5474d-124">Single</span></span>|<span data-ttu-id="5474d-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="5474d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5474d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="5474d-126">Relationships</span></span>
<span data-ttu-id="5474d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5474d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5474d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5474d-128">JSON Representation</span></span>
<span data-ttu-id="5474d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5474d-129">Here is a JSON representation of the resource.</span></span>
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



