---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb11f40faf9db58fefb984fcc08a9fedd66e97d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951548"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="0e040-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="0e040-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="0e040-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0e040-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e040-105">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0e040-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="0e040-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e040-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e040-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e040-107">Properties</span></span>
|<span data-ttu-id="0e040-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e040-108">Property</span></span>|<span data-ttu-id="0e040-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e040-109">Type</span></span>|<span data-ttu-id="0e040-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e040-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e040-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0e040-111">displayName</span></span>|<span data-ttu-id="0e040-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e040-112">String</span></span>|<span data-ttu-id="0e040-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0e040-113">Display Name.</span></span> <span data-ttu-id="0e040-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e040-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e040-115">descrição</span><span class="sxs-lookup"><span data-stu-id="0e040-115">description</span></span>|<span data-ttu-id="0e040-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e040-116">String</span></span>|<span data-ttu-id="0e040-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0e040-117">Description.</span></span> <span data-ttu-id="0e040-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e040-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e040-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0e040-119">omaUri</span></span>|<span data-ttu-id="0e040-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e040-120">String</span></span>|<span data-ttu-id="0e040-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0e040-121">OMA.</span></span> <span data-ttu-id="0e040-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e040-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e040-123">value</span><span class="sxs-lookup"><span data-stu-id="0e040-123">value</span></span>|<span data-ttu-id="0e040-124">Single</span><span class="sxs-lookup"><span data-stu-id="0e040-124">Single</span></span>|<span data-ttu-id="0e040-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="0e040-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e040-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0e040-126">Relationships</span></span>
<span data-ttu-id="0e040-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e040-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e040-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e040-128">JSON Representation</span></span>
<span data-ttu-id="0e040-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e040-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



