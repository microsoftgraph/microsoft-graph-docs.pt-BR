---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46bca1f6052dae3f4699b88258abce4b346c67bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868205"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="21fab-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="21fab-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="21fab-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21fab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21fab-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="21fab-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="21fab-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21fab-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21fab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21fab-107">Properties</span></span>
|<span data-ttu-id="21fab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21fab-108">Property</span></span>|<span data-ttu-id="21fab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="21fab-109">Type</span></span>|<span data-ttu-id="21fab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21fab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21fab-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21fab-111">displayName</span></span>|<span data-ttu-id="21fab-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21fab-112">String</span></span>|<span data-ttu-id="21fab-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="21fab-113">Display Name.</span></span> <span data-ttu-id="21fab-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21fab-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21fab-115">descrição</span><span class="sxs-lookup"><span data-stu-id="21fab-115">description</span></span>|<span data-ttu-id="21fab-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21fab-116">String</span></span>|<span data-ttu-id="21fab-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="21fab-117">Description.</span></span> <span data-ttu-id="21fab-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21fab-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21fab-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="21fab-119">omaUri</span></span>|<span data-ttu-id="21fab-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21fab-120">String</span></span>|<span data-ttu-id="21fab-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="21fab-121">OMA.</span></span> <span data-ttu-id="21fab-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21fab-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21fab-123">valor</span><span class="sxs-lookup"><span data-stu-id="21fab-123">value</span></span>|<span data-ttu-id="21fab-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="21fab-124">Boolean</span></span>|<span data-ttu-id="21fab-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="21fab-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21fab-126">Relações</span><span class="sxs-lookup"><span data-stu-id="21fab-126">Relationships</span></span>
<span data-ttu-id="21fab-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21fab-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21fab-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21fab-128">JSON Representation</span></span>
<span data-ttu-id="21fab-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21fab-129">Here is a JSON representation of the resource.</span></span>
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



