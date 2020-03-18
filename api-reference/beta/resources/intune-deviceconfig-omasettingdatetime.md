---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d4ade59cc6359f4cc9f5bd668882860cf49ff49
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788454"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="b178c-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="b178c-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="b178c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b178c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b178c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b178c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b178c-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b178c-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="b178c-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b178c-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b178c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b178c-108">Properties</span></span>
|<span data-ttu-id="b178c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b178c-109">Property</span></span>|<span data-ttu-id="b178c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b178c-110">Type</span></span>|<span data-ttu-id="b178c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b178c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b178c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b178c-112">displayName</span></span>|<span data-ttu-id="b178c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b178c-113">String</span></span>|<span data-ttu-id="b178c-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b178c-114">Display Name.</span></span> <span data-ttu-id="b178c-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b178c-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b178c-116">description</span><span class="sxs-lookup"><span data-stu-id="b178c-116">description</span></span>|<span data-ttu-id="b178c-117">String</span><span class="sxs-lookup"><span data-stu-id="b178c-117">String</span></span>|<span data-ttu-id="b178c-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b178c-118">Description.</span></span> <span data-ttu-id="b178c-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b178c-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b178c-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="b178c-120">omaUri</span></span>|<span data-ttu-id="b178c-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b178c-121">String</span></span>|<span data-ttu-id="b178c-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="b178c-122">OMA.</span></span> <span data-ttu-id="b178c-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b178c-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b178c-124">value</span><span class="sxs-lookup"><span data-stu-id="b178c-124">value</span></span>|<span data-ttu-id="b178c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b178c-125">DateTimeOffset</span></span>|<span data-ttu-id="b178c-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="b178c-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b178c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b178c-127">Relationships</span></span>
<span data-ttu-id="b178c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b178c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b178c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b178c-129">JSON Representation</span></span>
<span data-ttu-id="b178c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b178c-130">Here is a JSON representation of the resource.</span></span>
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



