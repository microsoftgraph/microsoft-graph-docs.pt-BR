---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0b3f2d04c9476cc10a67c1e68ba9a29288e8875
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986632"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="43bad-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="43bad-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="43bad-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43bad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43bad-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="43bad-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="43bad-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43bad-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43bad-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43bad-107">Properties</span></span>
|<span data-ttu-id="43bad-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43bad-108">Property</span></span>|<span data-ttu-id="43bad-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="43bad-109">Type</span></span>|<span data-ttu-id="43bad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43bad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43bad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="43bad-111">displayName</span></span>|<span data-ttu-id="43bad-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43bad-112">String</span></span>|<span data-ttu-id="43bad-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="43bad-113">Display Name.</span></span> <span data-ttu-id="43bad-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43bad-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43bad-115">descrição</span><span class="sxs-lookup"><span data-stu-id="43bad-115">description</span></span>|<span data-ttu-id="43bad-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43bad-116">String</span></span>|<span data-ttu-id="43bad-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="43bad-117">Description.</span></span> <span data-ttu-id="43bad-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43bad-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43bad-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="43bad-119">omaUri</span></span>|<span data-ttu-id="43bad-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43bad-120">String</span></span>|<span data-ttu-id="43bad-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="43bad-121">OMA.</span></span> <span data-ttu-id="43bad-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43bad-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43bad-123">valor</span><span class="sxs-lookup"><span data-stu-id="43bad-123">value</span></span>|<span data-ttu-id="43bad-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="43bad-124">Boolean</span></span>|<span data-ttu-id="43bad-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="43bad-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43bad-126">Relações</span><span class="sxs-lookup"><span data-stu-id="43bad-126">Relationships</span></span>
<span data-ttu-id="43bad-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43bad-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43bad-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43bad-128">JSON Representation</span></span>
<span data-ttu-id="43bad-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43bad-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



