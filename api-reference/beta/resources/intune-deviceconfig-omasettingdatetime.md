---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ce4123149be2faa89171e9a5eb1ba0ab6472515b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722968"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="53340-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="53340-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="53340-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53340-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53340-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53340-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53340-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53340-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53340-107">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="53340-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="53340-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53340-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53340-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53340-109">Properties</span></span>
|<span data-ttu-id="53340-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53340-110">Property</span></span>|<span data-ttu-id="53340-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="53340-111">Type</span></span>|<span data-ttu-id="53340-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="53340-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53340-113">displayName</span><span class="sxs-lookup"><span data-stu-id="53340-113">displayName</span></span>|<span data-ttu-id="53340-114">String</span><span class="sxs-lookup"><span data-stu-id="53340-114">String</span></span>|<span data-ttu-id="53340-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="53340-115">Display Name.</span></span> <span data-ttu-id="53340-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53340-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53340-117">description</span><span class="sxs-lookup"><span data-stu-id="53340-117">description</span></span>|<span data-ttu-id="53340-118">String</span><span class="sxs-lookup"><span data-stu-id="53340-118">String</span></span>|<span data-ttu-id="53340-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="53340-119">Description.</span></span> <span data-ttu-id="53340-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53340-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53340-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="53340-121">omaUri</span></span>|<span data-ttu-id="53340-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53340-122">String</span></span>|<span data-ttu-id="53340-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="53340-123">OMA.</span></span> <span data-ttu-id="53340-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="53340-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="53340-125">value</span><span class="sxs-lookup"><span data-stu-id="53340-125">value</span></span>|<span data-ttu-id="53340-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53340-126">DateTimeOffset</span></span>|<span data-ttu-id="53340-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="53340-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53340-128">Relações</span><span class="sxs-lookup"><span data-stu-id="53340-128">Relationships</span></span>
<span data-ttu-id="53340-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53340-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53340-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53340-130">JSON Representation</span></span>
<span data-ttu-id="53340-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53340-131">Here is a JSON representation of the resource.</span></span>
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





