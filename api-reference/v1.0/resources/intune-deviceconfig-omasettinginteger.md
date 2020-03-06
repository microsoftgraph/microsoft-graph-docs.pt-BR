---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7e9e45e6153d565c4d56a4112e5e00cafed04f46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532410"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="80098-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="80098-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="80098-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80098-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80098-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80098-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80098-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="80098-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="80098-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80098-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80098-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80098-108">Properties</span></span>
|<span data-ttu-id="80098-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80098-109">Property</span></span>|<span data-ttu-id="80098-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="80098-110">Type</span></span>|<span data-ttu-id="80098-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80098-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80098-112">displayName</span><span class="sxs-lookup"><span data-stu-id="80098-112">displayName</span></span>|<span data-ttu-id="80098-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80098-113">String</span></span>|<span data-ttu-id="80098-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="80098-114">Display Name.</span></span> <span data-ttu-id="80098-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80098-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80098-116">description</span><span class="sxs-lookup"><span data-stu-id="80098-116">description</span></span>|<span data-ttu-id="80098-117">String</span><span class="sxs-lookup"><span data-stu-id="80098-117">String</span></span>|<span data-ttu-id="80098-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="80098-118">Description.</span></span> <span data-ttu-id="80098-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80098-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80098-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="80098-120">omaUri</span></span>|<span data-ttu-id="80098-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80098-121">String</span></span>|<span data-ttu-id="80098-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="80098-122">OMA.</span></span> <span data-ttu-id="80098-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80098-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80098-124">valor</span><span class="sxs-lookup"><span data-stu-id="80098-124">value</span></span>|<span data-ttu-id="80098-125">Int32</span><span class="sxs-lookup"><span data-stu-id="80098-125">Int32</span></span>|<span data-ttu-id="80098-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="80098-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80098-127">Relações</span><span class="sxs-lookup"><span data-stu-id="80098-127">Relationships</span></span>
<span data-ttu-id="80098-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80098-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80098-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80098-129">JSON Representation</span></span>
<span data-ttu-id="80098-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80098-130">Here is a JSON representation of the resource.</span></span>
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




