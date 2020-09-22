---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17883b580671517bcdee88d95f1ac5a424e707da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073016"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="d242b-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="d242b-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="d242b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d242b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d242b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d242b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d242b-106">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="d242b-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="d242b-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d242b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d242b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d242b-108">Properties</span></span>
|<span data-ttu-id="d242b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d242b-109">Property</span></span>|<span data-ttu-id="d242b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d242b-110">Type</span></span>|<span data-ttu-id="d242b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d242b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d242b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d242b-112">displayName</span></span>|<span data-ttu-id="d242b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d242b-113">String</span></span>|<span data-ttu-id="d242b-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d242b-114">Display Name.</span></span> <span data-ttu-id="d242b-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d242b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d242b-116">description</span><span class="sxs-lookup"><span data-stu-id="d242b-116">description</span></span>|<span data-ttu-id="d242b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d242b-117">String</span></span>|<span data-ttu-id="d242b-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d242b-118">Description.</span></span> <span data-ttu-id="d242b-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d242b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d242b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d242b-120">omaUri</span></span>|<span data-ttu-id="d242b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d242b-121">String</span></span>|<span data-ttu-id="d242b-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d242b-122">OMA.</span></span> <span data-ttu-id="d242b-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d242b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d242b-124">value</span><span class="sxs-lookup"><span data-stu-id="d242b-124">value</span></span>|<span data-ttu-id="d242b-125">Single</span><span class="sxs-lookup"><span data-stu-id="d242b-125">Single</span></span>|<span data-ttu-id="d242b-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="d242b-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d242b-127">Relações</span><span class="sxs-lookup"><span data-stu-id="d242b-127">Relationships</span></span>
<span data-ttu-id="d242b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d242b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d242b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d242b-129">JSON Representation</span></span>
<span data-ttu-id="d242b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d242b-130">Here is a JSON representation of the resource.</span></span>
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









