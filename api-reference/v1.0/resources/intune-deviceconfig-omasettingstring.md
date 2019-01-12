---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0524e077c210f2b13744534b9f42b2bb19d6359b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911760"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="ae761-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="ae761-103">omaSettingString resource type</span></span>

> <span data-ttu-id="ae761-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ae761-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae761-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="ae761-105">OMA Settings String definition.</span></span>

<span data-ttu-id="ae761-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae761-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ae761-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae761-107">Properties</span></span>
|<span data-ttu-id="ae761-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae761-108">Property</span></span>|<span data-ttu-id="ae761-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae761-109">Type</span></span>|<span data-ttu-id="ae761-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae761-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae761-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ae761-111">displayName</span></span>|<span data-ttu-id="ae761-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae761-112">String</span></span>|<span data-ttu-id="ae761-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ae761-113">Display Name.</span></span> <span data-ttu-id="ae761-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae761-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ae761-115">descrição</span><span class="sxs-lookup"><span data-stu-id="ae761-115">description</span></span>|<span data-ttu-id="ae761-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae761-116">String</span></span>|<span data-ttu-id="ae761-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="ae761-117">Description.</span></span> <span data-ttu-id="ae761-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae761-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ae761-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ae761-119">omaUri</span></span>|<span data-ttu-id="ae761-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae761-120">String</span></span>|<span data-ttu-id="ae761-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ae761-121">OMA.</span></span> <span data-ttu-id="ae761-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ae761-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ae761-123">valor</span><span class="sxs-lookup"><span data-stu-id="ae761-123">value</span></span>|<span data-ttu-id="ae761-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae761-124">String</span></span>|<span data-ttu-id="ae761-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="ae761-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae761-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ae761-126">Relationships</span></span>
<span data-ttu-id="ae761-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae761-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae761-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae761-128">JSON Representation</span></span>
<span data-ttu-id="ae761-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae761-129">Here is a JSON representation of the resource.</span></span>
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



