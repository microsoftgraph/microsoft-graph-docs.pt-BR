---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb87ecf7f658e9eb6ed19904a09460d2b2695be4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172321"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="7b481-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="7b481-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="7b481-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b481-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b481-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b481-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b481-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="7b481-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="7b481-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7b481-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7b481-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b481-108">Properties</span></span>
|<span data-ttu-id="7b481-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b481-109">Property</span></span>|<span data-ttu-id="7b481-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b481-110">Type</span></span>|<span data-ttu-id="7b481-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b481-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b481-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7b481-112">displayName</span></span>|<span data-ttu-id="7b481-113">String</span><span class="sxs-lookup"><span data-stu-id="7b481-113">String</span></span>|<span data-ttu-id="7b481-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7b481-114">Display Name.</span></span> <span data-ttu-id="7b481-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7b481-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7b481-116">descrição</span><span class="sxs-lookup"><span data-stu-id="7b481-116">description</span></span>|<span data-ttu-id="7b481-117">String</span><span class="sxs-lookup"><span data-stu-id="7b481-117">String</span></span>|<span data-ttu-id="7b481-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="7b481-118">Description.</span></span> <span data-ttu-id="7b481-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7b481-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7b481-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="7b481-120">omaUri</span></span>|<span data-ttu-id="7b481-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b481-121">String</span></span>|<span data-ttu-id="7b481-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="7b481-122">OMA.</span></span> <span data-ttu-id="7b481-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7b481-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7b481-124">valor</span><span class="sxs-lookup"><span data-stu-id="7b481-124">value</span></span>|<span data-ttu-id="7b481-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7b481-125">Int32</span></span>|<span data-ttu-id="7b481-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="7b481-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b481-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7b481-127">Relationships</span></span>
<span data-ttu-id="7b481-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b481-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b481-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b481-129">JSON Representation</span></span>
<span data-ttu-id="7b481-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b481-130">Here is a JSON representation of the resource.</span></span>
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




