---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 9a525d031c9f24cf18495d83e22467e103bca6d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363687"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="e00a2-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="e00a2-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="e00a2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e00a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e00a2-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e00a2-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="e00a2-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e00a2-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e00a2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e00a2-107">Properties</span></span>
|<span data-ttu-id="e00a2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e00a2-108">Property</span></span>|<span data-ttu-id="e00a2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e00a2-109">Type</span></span>|<span data-ttu-id="e00a2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e00a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e00a2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e00a2-111">displayName</span></span>|<span data-ttu-id="e00a2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e00a2-112">String</span></span>|<span data-ttu-id="e00a2-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e00a2-113">Display Name.</span></span> <span data-ttu-id="e00a2-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e00a2-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e00a2-115">descrição</span><span class="sxs-lookup"><span data-stu-id="e00a2-115">description</span></span>|<span data-ttu-id="e00a2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e00a2-116">String</span></span>|<span data-ttu-id="e00a2-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e00a2-117">Description.</span></span> <span data-ttu-id="e00a2-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e00a2-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e00a2-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e00a2-119">omaUri</span></span>|<span data-ttu-id="e00a2-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e00a2-120">String</span></span>|<span data-ttu-id="e00a2-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="e00a2-121">OMA.</span></span> <span data-ttu-id="e00a2-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e00a2-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e00a2-123">value</span><span class="sxs-lookup"><span data-stu-id="e00a2-123">value</span></span>|<span data-ttu-id="e00a2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e00a2-124">DateTimeOffset</span></span>|<span data-ttu-id="e00a2-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="e00a2-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e00a2-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e00a2-126">Relationships</span></span>
<span data-ttu-id="e00a2-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e00a2-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e00a2-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e00a2-128">JSON Representation</span></span>
<span data-ttu-id="e00a2-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e00a2-129">Here is a JSON representation of the resource.</span></span>
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



