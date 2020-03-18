---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d20a88e79a1383789a67883d03aae6b8e4463f4e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788433"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="83210-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="83210-103">omaSettingString resource type</span></span>

> <span data-ttu-id="83210-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83210-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83210-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="83210-106">OMA Settings String definition.</span></span>


<span data-ttu-id="83210-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="83210-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="83210-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83210-108">Properties</span></span>
|<span data-ttu-id="83210-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83210-109">Property</span></span>|<span data-ttu-id="83210-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83210-110">Type</span></span>|<span data-ttu-id="83210-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83210-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83210-112">displayName</span><span class="sxs-lookup"><span data-stu-id="83210-112">displayName</span></span>|<span data-ttu-id="83210-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83210-113">String</span></span>|<span data-ttu-id="83210-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="83210-114">Display Name.</span></span> <span data-ttu-id="83210-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="83210-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="83210-116">description</span><span class="sxs-lookup"><span data-stu-id="83210-116">description</span></span>|<span data-ttu-id="83210-117">String</span><span class="sxs-lookup"><span data-stu-id="83210-117">String</span></span>|<span data-ttu-id="83210-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="83210-118">Description.</span></span> <span data-ttu-id="83210-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="83210-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="83210-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="83210-120">omaUri</span></span>|<span data-ttu-id="83210-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83210-121">String</span></span>|<span data-ttu-id="83210-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="83210-122">OMA.</span></span> <span data-ttu-id="83210-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="83210-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="83210-124">value</span><span class="sxs-lookup"><span data-stu-id="83210-124">value</span></span>|<span data-ttu-id="83210-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83210-125">String</span></span>|<span data-ttu-id="83210-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="83210-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83210-127">Relações</span><span class="sxs-lookup"><span data-stu-id="83210-127">Relationships</span></span>
<span data-ttu-id="83210-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83210-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83210-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83210-129">JSON Representation</span></span>
<span data-ttu-id="83210-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83210-130">Here is a JSON representation of the resource.</span></span>
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



