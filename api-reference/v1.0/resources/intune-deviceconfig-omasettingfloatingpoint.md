---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b5db5b376bdce3d428b36c014c949087ab36185
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473023"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="1ea21-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="1ea21-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="1ea21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ea21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ea21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ea21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ea21-106">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1ea21-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="1ea21-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ea21-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ea21-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ea21-108">Properties</span></span>
|<span data-ttu-id="1ea21-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ea21-109">Property</span></span>|<span data-ttu-id="1ea21-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ea21-110">Type</span></span>|<span data-ttu-id="1ea21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea21-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1ea21-112">displayName</span></span>|<span data-ttu-id="1ea21-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ea21-113">String</span></span>|<span data-ttu-id="1ea21-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1ea21-114">Display Name.</span></span> <span data-ttu-id="1ea21-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ea21-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ea21-116">description</span><span class="sxs-lookup"><span data-stu-id="1ea21-116">description</span></span>|<span data-ttu-id="1ea21-117">String</span><span class="sxs-lookup"><span data-stu-id="1ea21-117">String</span></span>|<span data-ttu-id="1ea21-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1ea21-118">Description.</span></span> <span data-ttu-id="1ea21-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ea21-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ea21-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="1ea21-120">omaUri</span></span>|<span data-ttu-id="1ea21-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ea21-121">String</span></span>|<span data-ttu-id="1ea21-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="1ea21-122">OMA.</span></span> <span data-ttu-id="1ea21-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ea21-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1ea21-124">value</span><span class="sxs-lookup"><span data-stu-id="1ea21-124">value</span></span>|<span data-ttu-id="1ea21-125">Single</span><span class="sxs-lookup"><span data-stu-id="1ea21-125">Single</span></span>|<span data-ttu-id="1ea21-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="1ea21-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ea21-127">Relações</span><span class="sxs-lookup"><span data-stu-id="1ea21-127">Relationships</span></span>
<span data-ttu-id="1ea21-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ea21-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ea21-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ea21-129">JSON Representation</span></span>
<span data-ttu-id="1ea21-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ea21-130">Here is a JSON representation of the resource.</span></span>
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







