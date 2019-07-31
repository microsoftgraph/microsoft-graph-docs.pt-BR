---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4abe8f9b22cdc75e8e560ddb9e15a75425cb3f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011411"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="99f42-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="99f42-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="99f42-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99f42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99f42-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99f42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99f42-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="99f42-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="99f42-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99f42-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99f42-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99f42-108">Properties</span></span>
|<span data-ttu-id="99f42-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99f42-109">Property</span></span>|<span data-ttu-id="99f42-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="99f42-110">Type</span></span>|<span data-ttu-id="99f42-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99f42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f42-112">displayName</span><span class="sxs-lookup"><span data-stu-id="99f42-112">displayName</span></span>|<span data-ttu-id="99f42-113">String</span><span class="sxs-lookup"><span data-stu-id="99f42-113">String</span></span>|<span data-ttu-id="99f42-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="99f42-114">Display Name.</span></span> <span data-ttu-id="99f42-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99f42-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99f42-116">descrição</span><span class="sxs-lookup"><span data-stu-id="99f42-116">description</span></span>|<span data-ttu-id="99f42-117">String</span><span class="sxs-lookup"><span data-stu-id="99f42-117">String</span></span>|<span data-ttu-id="99f42-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="99f42-118">Description.</span></span> <span data-ttu-id="99f42-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99f42-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99f42-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="99f42-120">omaUri</span></span>|<span data-ttu-id="99f42-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99f42-121">String</span></span>|<span data-ttu-id="99f42-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="99f42-122">OMA.</span></span> <span data-ttu-id="99f42-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99f42-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99f42-124">value</span><span class="sxs-lookup"><span data-stu-id="99f42-124">value</span></span>|<span data-ttu-id="99f42-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f42-125">DateTimeOffset</span></span>|<span data-ttu-id="99f42-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="99f42-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99f42-127">Relações</span><span class="sxs-lookup"><span data-stu-id="99f42-127">Relationships</span></span>
<span data-ttu-id="99f42-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99f42-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99f42-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99f42-129">JSON Representation</span></span>
<span data-ttu-id="99f42-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99f42-130">Here is a JSON representation of the resource.</span></span>
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





