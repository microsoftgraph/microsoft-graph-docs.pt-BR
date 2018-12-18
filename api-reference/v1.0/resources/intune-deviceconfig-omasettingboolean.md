---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 10101217d1c0f07931cb847e1c14f36844c8dc9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323279"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="42e78-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="42e78-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="42e78-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42e78-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42e78-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="42e78-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="42e78-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42e78-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42e78-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42e78-107">Properties</span></span>
|<span data-ttu-id="42e78-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42e78-108">Property</span></span>|<span data-ttu-id="42e78-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="42e78-109">Type</span></span>|<span data-ttu-id="42e78-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="42e78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42e78-111">displayName</span><span class="sxs-lookup"><span data-stu-id="42e78-111">displayName</span></span>|<span data-ttu-id="42e78-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42e78-112">String</span></span>|<span data-ttu-id="42e78-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="42e78-113">Display Name.</span></span> <span data-ttu-id="42e78-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42e78-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42e78-115">descrição</span><span class="sxs-lookup"><span data-stu-id="42e78-115">description</span></span>|<span data-ttu-id="42e78-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42e78-116">String</span></span>|<span data-ttu-id="42e78-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="42e78-117">Description.</span></span> <span data-ttu-id="42e78-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42e78-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42e78-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="42e78-119">omaUri</span></span>|<span data-ttu-id="42e78-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42e78-120">String</span></span>|<span data-ttu-id="42e78-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="42e78-121">OMA.</span></span> <span data-ttu-id="42e78-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42e78-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42e78-123">valor</span><span class="sxs-lookup"><span data-stu-id="42e78-123">value</span></span>|<span data-ttu-id="42e78-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="42e78-124">Boolean</span></span>|<span data-ttu-id="42e78-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="42e78-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42e78-126">Relações</span><span class="sxs-lookup"><span data-stu-id="42e78-126">Relationships</span></span>
<span data-ttu-id="42e78-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42e78-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42e78-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42e78-128">JSON Representation</span></span>
<span data-ttu-id="42e78-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42e78-129">Here is a JSON representation of the resource.</span></span>
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



