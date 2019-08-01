---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 122a8fd7ffdef7d314e16bf6154838e09598f7d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031315"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="a9689-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="a9689-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="a9689-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9689-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9689-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a9689-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="a9689-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9689-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9689-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9689-107">Properties</span></span>
|<span data-ttu-id="a9689-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9689-108">Property</span></span>|<span data-ttu-id="a9689-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9689-109">Type</span></span>|<span data-ttu-id="a9689-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9689-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9689-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a9689-111">displayName</span></span>|<span data-ttu-id="a9689-112">String</span><span class="sxs-lookup"><span data-stu-id="a9689-112">String</span></span>|<span data-ttu-id="a9689-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a9689-113">Display Name.</span></span> <span data-ttu-id="a9689-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9689-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9689-115">descrição</span><span class="sxs-lookup"><span data-stu-id="a9689-115">description</span></span>|<span data-ttu-id="a9689-116">String</span><span class="sxs-lookup"><span data-stu-id="a9689-116">String</span></span>|<span data-ttu-id="a9689-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a9689-117">Description.</span></span> <span data-ttu-id="a9689-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9689-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9689-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a9689-119">omaUri</span></span>|<span data-ttu-id="a9689-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9689-120">String</span></span>|<span data-ttu-id="a9689-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="a9689-121">OMA.</span></span> <span data-ttu-id="a9689-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9689-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9689-123">value</span><span class="sxs-lookup"><span data-stu-id="a9689-123">value</span></span>|<span data-ttu-id="a9689-124">Single</span><span class="sxs-lookup"><span data-stu-id="a9689-124">Single</span></span>|<span data-ttu-id="a9689-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="a9689-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9689-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a9689-126">Relationships</span></span>
<span data-ttu-id="a9689-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9689-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9689-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9689-128">JSON Representation</span></span>
<span data-ttu-id="a9689-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9689-129">Here is a JSON representation of the resource.</span></span>
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



