---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 6a2e6fe6e6782159afa99d91785ae9e854a2e99c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306549"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="ce75f-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="ce75f-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="ce75f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce75f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce75f-105">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="ce75f-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="ce75f-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce75f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce75f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce75f-107">Properties</span></span>
|<span data-ttu-id="ce75f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce75f-108">Property</span></span>|<span data-ttu-id="ce75f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce75f-109">Type</span></span>|<span data-ttu-id="ce75f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce75f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce75f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ce75f-111">displayName</span></span>|<span data-ttu-id="ce75f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce75f-112">String</span></span>|<span data-ttu-id="ce75f-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ce75f-113">Display Name.</span></span> <span data-ttu-id="ce75f-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce75f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce75f-115">descrição</span><span class="sxs-lookup"><span data-stu-id="ce75f-115">description</span></span>|<span data-ttu-id="ce75f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce75f-116">String</span></span>|<span data-ttu-id="ce75f-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="ce75f-117">Description.</span></span> <span data-ttu-id="ce75f-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce75f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce75f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ce75f-119">omaUri</span></span>|<span data-ttu-id="ce75f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce75f-120">String</span></span>|<span data-ttu-id="ce75f-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ce75f-121">OMA.</span></span> <span data-ttu-id="ce75f-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce75f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce75f-123">valor</span><span class="sxs-lookup"><span data-stu-id="ce75f-123">value</span></span>|<span data-ttu-id="ce75f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ce75f-124">Int32</span></span>|<span data-ttu-id="ce75f-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="ce75f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce75f-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ce75f-126">Relationships</span></span>
<span data-ttu-id="ce75f-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce75f-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce75f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce75f-128">JSON Representation</span></span>
<span data-ttu-id="ce75f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce75f-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



