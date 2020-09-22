---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6291fc5b81de9dea1bfa67515f4df296d9e3001e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978150"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="f8e34-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="f8e34-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="f8e34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8e34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8e34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e34-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f8e34-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="f8e34-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f8e34-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8e34-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8e34-108">Properties</span></span>
|<span data-ttu-id="f8e34-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8e34-109">Property</span></span>|<span data-ttu-id="f8e34-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8e34-110">Type</span></span>|<span data-ttu-id="f8e34-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8e34-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f8e34-112">displayName</span></span>|<span data-ttu-id="f8e34-113">String</span><span class="sxs-lookup"><span data-stu-id="f8e34-113">String</span></span>|<span data-ttu-id="f8e34-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f8e34-114">Display Name.</span></span> <span data-ttu-id="f8e34-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f8e34-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f8e34-116">description</span><span class="sxs-lookup"><span data-stu-id="f8e34-116">description</span></span>|<span data-ttu-id="f8e34-117">String</span><span class="sxs-lookup"><span data-stu-id="f8e34-117">String</span></span>|<span data-ttu-id="f8e34-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f8e34-118">Description.</span></span> <span data-ttu-id="f8e34-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f8e34-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f8e34-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f8e34-120">omaUri</span></span>|<span data-ttu-id="f8e34-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8e34-121">String</span></span>|<span data-ttu-id="f8e34-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="f8e34-122">OMA.</span></span> <span data-ttu-id="f8e34-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f8e34-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f8e34-124">value</span><span class="sxs-lookup"><span data-stu-id="f8e34-124">value</span></span>|<span data-ttu-id="f8e34-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8e34-125">DateTimeOffset</span></span>|<span data-ttu-id="f8e34-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="f8e34-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8e34-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f8e34-127">Relationships</span></span>
<span data-ttu-id="f8e34-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8e34-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8e34-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8e34-129">JSON Representation</span></span>
<span data-ttu-id="f8e34-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8e34-130">Here is a JSON representation of the resource.</span></span>
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









