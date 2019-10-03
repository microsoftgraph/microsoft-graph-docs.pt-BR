---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a93824eec0df18984809b0580c4a1dcb5caec55
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366570"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="64822-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="64822-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="64822-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64822-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64822-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="64822-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="64822-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="64822-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64822-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64822-107">Properties</span></span>
|<span data-ttu-id="64822-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64822-108">Property</span></span>|<span data-ttu-id="64822-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="64822-109">Type</span></span>|<span data-ttu-id="64822-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="64822-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64822-111">displayName</span><span class="sxs-lookup"><span data-stu-id="64822-111">displayName</span></span>|<span data-ttu-id="64822-112">String</span><span class="sxs-lookup"><span data-stu-id="64822-112">String</span></span>|<span data-ttu-id="64822-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="64822-113">Display Name.</span></span> <span data-ttu-id="64822-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="64822-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="64822-115">descrição</span><span class="sxs-lookup"><span data-stu-id="64822-115">description</span></span>|<span data-ttu-id="64822-116">String</span><span class="sxs-lookup"><span data-stu-id="64822-116">String</span></span>|<span data-ttu-id="64822-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="64822-117">Description.</span></span> <span data-ttu-id="64822-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="64822-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="64822-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="64822-119">omaUri</span></span>|<span data-ttu-id="64822-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64822-120">String</span></span>|<span data-ttu-id="64822-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="64822-121">OMA.</span></span> <span data-ttu-id="64822-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="64822-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="64822-123">value</span><span class="sxs-lookup"><span data-stu-id="64822-123">value</span></span>|<span data-ttu-id="64822-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="64822-124">Boolean</span></span>|<span data-ttu-id="64822-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="64822-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64822-126">Relações</span><span class="sxs-lookup"><span data-stu-id="64822-126">Relationships</span></span>
<span data-ttu-id="64822-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64822-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64822-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64822-128">JSON Representation</span></span>
<span data-ttu-id="64822-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64822-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




