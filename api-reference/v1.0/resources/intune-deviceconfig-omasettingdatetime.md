---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: afd66ce8838abc3ade8857ec5a4bda74144d6792
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865175"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="8ed8c-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed8c-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="8ed8c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ed8c-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="8ed8c-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ed8c-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ed8c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ed8c-107">Properties</span></span>
|<span data-ttu-id="8ed8c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ed8c-108">Property</span></span>|<span data-ttu-id="8ed8c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ed8c-109">Type</span></span>|<span data-ttu-id="8ed8c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ed8c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8ed8c-111">displayName</span></span>|<span data-ttu-id="8ed8c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ed8c-112">String</span></span>|<span data-ttu-id="8ed8c-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-113">Display Name.</span></span> <span data-ttu-id="8ed8c-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ed8c-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ed8c-115">descrição</span><span class="sxs-lookup"><span data-stu-id="8ed8c-115">description</span></span>|<span data-ttu-id="8ed8c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ed8c-116">String</span></span>|<span data-ttu-id="8ed8c-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-117">Description.</span></span> <span data-ttu-id="8ed8c-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ed8c-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ed8c-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8ed8c-119">omaUri</span></span>|<span data-ttu-id="8ed8c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ed8c-120">String</span></span>|<span data-ttu-id="8ed8c-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-121">OMA.</span></span> <span data-ttu-id="8ed8c-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ed8c-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ed8c-123">value</span><span class="sxs-lookup"><span data-stu-id="8ed8c-123">value</span></span>|<span data-ttu-id="8ed8c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed8c-124">DateTimeOffset</span></span>|<span data-ttu-id="8ed8c-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ed8c-126">Relações</span><span class="sxs-lookup"><span data-stu-id="8ed8c-126">Relationships</span></span>
<span data-ttu-id="8ed8c-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ed8c-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ed8c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ed8c-128">JSON Representation</span></span>
<span data-ttu-id="8ed8c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-129">Here is a JSON representation of the resource.</span></span>
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



