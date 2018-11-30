---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
ms.openlocfilehash: 36c22b423161d9f3c58c3085fb7b040c663d460b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006927"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="4b2a3-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="4b2a3-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="4b2a3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b2a3-105">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="4b2a3-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b2a3-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b2a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b2a3-107">Properties</span></span>
|<span data-ttu-id="4b2a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b2a3-108">Property</span></span>|<span data-ttu-id="4b2a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b2a3-109">Type</span></span>|<span data-ttu-id="4b2a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b2a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b2a3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4b2a3-111">displayName</span></span>|<span data-ttu-id="4b2a3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b2a3-112">String</span></span>|<span data-ttu-id="4b2a3-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-113">Display Name.</span></span> <span data-ttu-id="4b2a3-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b2a3-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b2a3-115">descrição</span><span class="sxs-lookup"><span data-stu-id="4b2a3-115">description</span></span>|<span data-ttu-id="4b2a3-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b2a3-116">String</span></span>|<span data-ttu-id="4b2a3-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-117">Description.</span></span> <span data-ttu-id="4b2a3-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b2a3-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b2a3-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4b2a3-119">omaUri</span></span>|<span data-ttu-id="4b2a3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b2a3-120">String</span></span>|<span data-ttu-id="4b2a3-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-121">OMA.</span></span> <span data-ttu-id="4b2a3-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b2a3-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b2a3-123">valor</span><span class="sxs-lookup"><span data-stu-id="4b2a3-123">value</span></span>|<span data-ttu-id="4b2a3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4b2a3-124">Int32</span></span>|<span data-ttu-id="4b2a3-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b2a3-126">Relações</span><span class="sxs-lookup"><span data-stu-id="4b2a3-126">Relationships</span></span>
<span data-ttu-id="4b2a3-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b2a3-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b2a3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b2a3-128">JSON Representation</span></span>
<span data-ttu-id="4b2a3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b2a3-129">Here is a JSON representation of the resource.</span></span>
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



