---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cf2e556fe434a7a0ab8baa4d42a4098e66c698cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473001"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="f098d-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="f098d-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="f098d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f098d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f098d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f098d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f098d-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f098d-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="f098d-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f098d-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f098d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f098d-108">Properties</span></span>
|<span data-ttu-id="f098d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f098d-109">Property</span></span>|<span data-ttu-id="f098d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f098d-110">Type</span></span>|<span data-ttu-id="f098d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f098d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f098d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f098d-112">displayName</span></span>|<span data-ttu-id="f098d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f098d-113">String</span></span>|<span data-ttu-id="f098d-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f098d-114">Display Name.</span></span> <span data-ttu-id="f098d-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f098d-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f098d-116">description</span><span class="sxs-lookup"><span data-stu-id="f098d-116">description</span></span>|<span data-ttu-id="f098d-117">String</span><span class="sxs-lookup"><span data-stu-id="f098d-117">String</span></span>|<span data-ttu-id="f098d-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f098d-118">Description.</span></span> <span data-ttu-id="f098d-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f098d-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f098d-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f098d-120">omaUri</span></span>|<span data-ttu-id="f098d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f098d-121">String</span></span>|<span data-ttu-id="f098d-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="f098d-122">OMA.</span></span> <span data-ttu-id="f098d-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f098d-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f098d-124">valor</span><span class="sxs-lookup"><span data-stu-id="f098d-124">value</span></span>|<span data-ttu-id="f098d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f098d-125">Int32</span></span>|<span data-ttu-id="f098d-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="f098d-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f098d-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f098d-127">Relationships</span></span>
<span data-ttu-id="f098d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f098d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f098d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f098d-129">JSON Representation</span></span>
<span data-ttu-id="f098d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f098d-130">Here is a JSON representation of the resource.</span></span>
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







