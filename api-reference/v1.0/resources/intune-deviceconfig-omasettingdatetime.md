---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99fa5ccf0b26ebd04ce232eb8bf4df9a9d4ace81
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755879"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d6414-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="d6414-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="d6414-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6414-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6414-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6414-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6414-106">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="d6414-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="d6414-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6414-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6414-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6414-108">Properties</span></span>
|<span data-ttu-id="d6414-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6414-109">Property</span></span>|<span data-ttu-id="d6414-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6414-110">Type</span></span>|<span data-ttu-id="d6414-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6414-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6414-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d6414-112">displayName</span></span>|<span data-ttu-id="d6414-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6414-113">String</span></span>|<span data-ttu-id="d6414-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d6414-114">Display Name.</span></span> <span data-ttu-id="d6414-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6414-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6414-116">descrição</span><span class="sxs-lookup"><span data-stu-id="d6414-116">description</span></span>|<span data-ttu-id="d6414-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6414-117">String</span></span>|<span data-ttu-id="d6414-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d6414-118">Description.</span></span> <span data-ttu-id="d6414-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6414-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6414-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d6414-120">omaUri</span></span>|<span data-ttu-id="d6414-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6414-121">String</span></span>|<span data-ttu-id="d6414-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d6414-122">OMA.</span></span> <span data-ttu-id="d6414-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6414-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6414-124">value</span><span class="sxs-lookup"><span data-stu-id="d6414-124">value</span></span>|<span data-ttu-id="d6414-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6414-125">DateTimeOffset</span></span>|<span data-ttu-id="d6414-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="d6414-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6414-127">Relações</span><span class="sxs-lookup"><span data-stu-id="d6414-127">Relationships</span></span>
<span data-ttu-id="d6414-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d6414-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6414-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6414-129">JSON Representation</span></span>
<span data-ttu-id="d6414-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6414-130">Here is a JSON representation of the resource.</span></span>
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




