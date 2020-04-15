---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d8d9151ad40ef42ca24730197cdebe882eccb97
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473038"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0a077-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="0a077-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="0a077-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a077-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a077-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a077-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0a077-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="0a077-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a077-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a077-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a077-108">Properties</span></span>
|<span data-ttu-id="0a077-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a077-109">Property</span></span>|<span data-ttu-id="0a077-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a077-110">Type</span></span>|<span data-ttu-id="0a077-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a077-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a077-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0a077-112">displayName</span></span>|<span data-ttu-id="0a077-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a077-113">String</span></span>|<span data-ttu-id="0a077-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0a077-114">Display Name.</span></span> <span data-ttu-id="0a077-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a077-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0a077-116">description</span><span class="sxs-lookup"><span data-stu-id="0a077-116">description</span></span>|<span data-ttu-id="0a077-117">String</span><span class="sxs-lookup"><span data-stu-id="0a077-117">String</span></span>|<span data-ttu-id="0a077-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0a077-118">Description.</span></span> <span data-ttu-id="0a077-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a077-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0a077-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="0a077-120">omaUri</span></span>|<span data-ttu-id="0a077-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a077-121">String</span></span>|<span data-ttu-id="0a077-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="0a077-122">OMA.</span></span> <span data-ttu-id="0a077-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0a077-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0a077-124">value</span><span class="sxs-lookup"><span data-stu-id="0a077-124">value</span></span>|<span data-ttu-id="0a077-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a077-125">DateTimeOffset</span></span>|<span data-ttu-id="0a077-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="0a077-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a077-127">Relações</span><span class="sxs-lookup"><span data-stu-id="0a077-127">Relationships</span></span>
<span data-ttu-id="0a077-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a077-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a077-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a077-129">JSON Representation</span></span>
<span data-ttu-id="0a077-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a077-130">Here is a JSON representation of the resource.</span></span>
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







