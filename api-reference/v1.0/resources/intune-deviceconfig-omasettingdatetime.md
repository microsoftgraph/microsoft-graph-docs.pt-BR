---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
ms.openlocfilehash: b4ea11c22acb2a4119c2de1934f1ae66c2310658
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004142"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="8f466-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="8f466-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="8f466-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f466-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f466-105">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="8f466-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="8f466-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f466-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f466-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f466-107">Properties</span></span>
|<span data-ttu-id="8f466-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f466-108">Property</span></span>|<span data-ttu-id="8f466-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f466-109">Type</span></span>|<span data-ttu-id="8f466-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f466-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f466-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8f466-111">displayName</span></span>|<span data-ttu-id="8f466-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f466-112">String</span></span>|<span data-ttu-id="8f466-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="8f466-113">Display Name.</span></span> <span data-ttu-id="8f466-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f466-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f466-115">descrição</span><span class="sxs-lookup"><span data-stu-id="8f466-115">description</span></span>|<span data-ttu-id="8f466-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f466-116">String</span></span>|<span data-ttu-id="8f466-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="8f466-117">Description.</span></span> <span data-ttu-id="8f466-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f466-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f466-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8f466-119">omaUri</span></span>|<span data-ttu-id="8f466-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f466-120">String</span></span>|<span data-ttu-id="8f466-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8f466-121">OMA.</span></span> <span data-ttu-id="8f466-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f466-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f466-123">value</span><span class="sxs-lookup"><span data-stu-id="8f466-123">value</span></span>|<span data-ttu-id="8f466-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f466-124">DateTimeOffset</span></span>|<span data-ttu-id="8f466-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="8f466-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f466-126">Relações</span><span class="sxs-lookup"><span data-stu-id="8f466-126">Relationships</span></span>
<span data-ttu-id="8f466-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f466-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f466-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f466-128">JSON Representation</span></span>
<span data-ttu-id="8f466-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f466-129">Here is a JSON representation of the resource.</span></span>
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



