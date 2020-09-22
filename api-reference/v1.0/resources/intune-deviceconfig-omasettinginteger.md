---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46406b403dd700ee7e8517c10956f310957dcaf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978157"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="f0891-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="f0891-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="f0891-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0891-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0891-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0891-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0891-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f0891-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="f0891-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0891-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0891-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0891-108">Properties</span></span>
|<span data-ttu-id="f0891-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0891-109">Property</span></span>|<span data-ttu-id="f0891-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0891-110">Type</span></span>|<span data-ttu-id="f0891-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0891-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0891-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f0891-112">displayName</span></span>|<span data-ttu-id="f0891-113">String</span><span class="sxs-lookup"><span data-stu-id="f0891-113">String</span></span>|<span data-ttu-id="f0891-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f0891-114">Display Name.</span></span> <span data-ttu-id="f0891-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0891-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0891-116">description</span><span class="sxs-lookup"><span data-stu-id="f0891-116">description</span></span>|<span data-ttu-id="f0891-117">String</span><span class="sxs-lookup"><span data-stu-id="f0891-117">String</span></span>|<span data-ttu-id="f0891-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f0891-118">Description.</span></span> <span data-ttu-id="f0891-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0891-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0891-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f0891-120">omaUri</span></span>|<span data-ttu-id="f0891-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0891-121">String</span></span>|<span data-ttu-id="f0891-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="f0891-122">OMA.</span></span> <span data-ttu-id="f0891-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0891-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0891-124">valor</span><span class="sxs-lookup"><span data-stu-id="f0891-124">value</span></span>|<span data-ttu-id="f0891-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f0891-125">Int32</span></span>|<span data-ttu-id="f0891-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="f0891-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0891-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f0891-127">Relationships</span></span>
<span data-ttu-id="f0891-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0891-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0891-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0891-129">JSON Representation</span></span>
<span data-ttu-id="f0891-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0891-130">Here is a JSON representation of the resource.</span></span>
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









