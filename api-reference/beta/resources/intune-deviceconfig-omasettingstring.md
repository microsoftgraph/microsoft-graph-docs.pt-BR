---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22c69270126349d8d1d4afca4555abd18768aa3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803028"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="45f80-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="45f80-103">omaSettingString resource type</span></span>

> <span data-ttu-id="45f80-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45f80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45f80-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45f80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f80-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="45f80-106">OMA Settings String definition.</span></span>


<span data-ttu-id="45f80-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45f80-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45f80-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45f80-108">Properties</span></span>
|<span data-ttu-id="45f80-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45f80-109">Property</span></span>|<span data-ttu-id="45f80-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="45f80-110">Type</span></span>|<span data-ttu-id="45f80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f80-112">displayName</span><span class="sxs-lookup"><span data-stu-id="45f80-112">displayName</span></span>|<span data-ttu-id="45f80-113">String</span><span class="sxs-lookup"><span data-stu-id="45f80-113">String</span></span>|<span data-ttu-id="45f80-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="45f80-114">Display Name.</span></span> <span data-ttu-id="45f80-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45f80-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45f80-116">description</span><span class="sxs-lookup"><span data-stu-id="45f80-116">description</span></span>|<span data-ttu-id="45f80-117">String</span><span class="sxs-lookup"><span data-stu-id="45f80-117">String</span></span>|<span data-ttu-id="45f80-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="45f80-118">Description.</span></span> <span data-ttu-id="45f80-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45f80-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45f80-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="45f80-120">omaUri</span></span>|<span data-ttu-id="45f80-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45f80-121">String</span></span>|<span data-ttu-id="45f80-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="45f80-122">OMA.</span></span> <span data-ttu-id="45f80-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45f80-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45f80-124">value</span><span class="sxs-lookup"><span data-stu-id="45f80-124">value</span></span>|<span data-ttu-id="45f80-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45f80-125">String</span></span>|<span data-ttu-id="45f80-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="45f80-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45f80-127">Relações</span><span class="sxs-lookup"><span data-stu-id="45f80-127">Relationships</span></span>
<span data-ttu-id="45f80-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="45f80-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45f80-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45f80-129">JSON Representation</span></span>
<span data-ttu-id="45f80-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45f80-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```





