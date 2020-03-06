---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a48686bc0b92d7b428fd0a6332080811b2726aff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530584"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="446d8-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="446d8-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="446d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="446d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="446d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="446d8-106">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="446d8-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="446d8-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="446d8-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="446d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="446d8-108">Properties</span></span>
|<span data-ttu-id="446d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="446d8-109">Property</span></span>|<span data-ttu-id="446d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="446d8-110">Type</span></span>|<span data-ttu-id="446d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="446d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="446d8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="446d8-112">displayName</span></span>|<span data-ttu-id="446d8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d8-113">String</span></span>|<span data-ttu-id="446d8-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="446d8-114">Display Name.</span></span> <span data-ttu-id="446d8-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="446d8-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="446d8-116">description</span><span class="sxs-lookup"><span data-stu-id="446d8-116">description</span></span>|<span data-ttu-id="446d8-117">String</span><span class="sxs-lookup"><span data-stu-id="446d8-117">String</span></span>|<span data-ttu-id="446d8-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="446d8-118">Description.</span></span> <span data-ttu-id="446d8-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="446d8-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="446d8-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="446d8-120">omaUri</span></span>|<span data-ttu-id="446d8-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d8-121">String</span></span>|<span data-ttu-id="446d8-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="446d8-122">OMA.</span></span> <span data-ttu-id="446d8-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="446d8-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="446d8-124">value</span><span class="sxs-lookup"><span data-stu-id="446d8-124">value</span></span>|<span data-ttu-id="446d8-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="446d8-125">Boolean</span></span>|<span data-ttu-id="446d8-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="446d8-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="446d8-127">Relações</span><span class="sxs-lookup"><span data-stu-id="446d8-127">Relationships</span></span>
<span data-ttu-id="446d8-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446d8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="446d8-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="446d8-129">JSON Representation</span></span>
<span data-ttu-id="446d8-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="446d8-130">Here is a JSON representation of the resource.</span></span>
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




