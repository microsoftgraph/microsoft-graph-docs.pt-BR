---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71347ecd4a566409d1043c788df70601ffc70a2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028025"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0de55-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="0de55-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="0de55-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0de55-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0de55-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0de55-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="0de55-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0de55-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0de55-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0de55-107">Properties</span></span>
|<span data-ttu-id="0de55-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0de55-108">Property</span></span>|<span data-ttu-id="0de55-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0de55-109">Type</span></span>|<span data-ttu-id="0de55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0de55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de55-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0de55-111">displayName</span></span>|<span data-ttu-id="0de55-112">String</span><span class="sxs-lookup"><span data-stu-id="0de55-112">String</span></span>|<span data-ttu-id="0de55-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0de55-113">Display Name.</span></span> <span data-ttu-id="0de55-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0de55-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0de55-115">descrição</span><span class="sxs-lookup"><span data-stu-id="0de55-115">description</span></span>|<span data-ttu-id="0de55-116">String</span><span class="sxs-lookup"><span data-stu-id="0de55-116">String</span></span>|<span data-ttu-id="0de55-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0de55-117">Description.</span></span> <span data-ttu-id="0de55-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0de55-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0de55-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0de55-119">omaUri</span></span>|<span data-ttu-id="0de55-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0de55-120">String</span></span>|<span data-ttu-id="0de55-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0de55-121">OMA.</span></span> <span data-ttu-id="0de55-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0de55-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0de55-123">value</span><span class="sxs-lookup"><span data-stu-id="0de55-123">value</span></span>|<span data-ttu-id="0de55-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0de55-124">DateTimeOffset</span></span>|<span data-ttu-id="0de55-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="0de55-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0de55-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0de55-126">Relationships</span></span>
<span data-ttu-id="0de55-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0de55-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0de55-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0de55-128">JSON Representation</span></span>
<span data-ttu-id="0de55-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0de55-129">Here is a JSON representation of the resource.</span></span>
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



