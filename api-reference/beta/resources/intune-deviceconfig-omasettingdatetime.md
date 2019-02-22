---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 283b41018ad89b157c679c8b532c869d350b9182
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144461"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="bb15a-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="bb15a-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="bb15a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb15a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb15a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb15a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb15a-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="bb15a-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="bb15a-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bb15a-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb15a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb15a-108">Properties</span></span>
|<span data-ttu-id="bb15a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb15a-109">Property</span></span>|<span data-ttu-id="bb15a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb15a-110">Type</span></span>|<span data-ttu-id="bb15a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb15a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb15a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bb15a-112">displayName</span></span>|<span data-ttu-id="bb15a-113">String</span><span class="sxs-lookup"><span data-stu-id="bb15a-113">String</span></span>|<span data-ttu-id="bb15a-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="bb15a-114">Display Name.</span></span> <span data-ttu-id="bb15a-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bb15a-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bb15a-116">descrição</span><span class="sxs-lookup"><span data-stu-id="bb15a-116">description</span></span>|<span data-ttu-id="bb15a-117">String</span><span class="sxs-lookup"><span data-stu-id="bb15a-117">String</span></span>|<span data-ttu-id="bb15a-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="bb15a-118">Description.</span></span> <span data-ttu-id="bb15a-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bb15a-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bb15a-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="bb15a-120">omaUri</span></span>|<span data-ttu-id="bb15a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb15a-121">String</span></span>|<span data-ttu-id="bb15a-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="bb15a-122">OMA.</span></span> <span data-ttu-id="bb15a-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bb15a-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bb15a-124">value</span><span class="sxs-lookup"><span data-stu-id="bb15a-124">value</span></span>|<span data-ttu-id="bb15a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb15a-125">DateTimeOffset</span></span>|<span data-ttu-id="bb15a-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="bb15a-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb15a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="bb15a-127">Relationships</span></span>
<span data-ttu-id="bb15a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb15a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb15a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb15a-129">JSON Representation</span></span>
<span data-ttu-id="bb15a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb15a-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```




