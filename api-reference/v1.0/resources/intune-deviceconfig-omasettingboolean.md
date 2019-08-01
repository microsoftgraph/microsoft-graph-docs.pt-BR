---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0ecb59f45a83cc98c6ff060b46ba0c620dc9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031336"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="6e0ba-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="6e0ba-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="6e0ba-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e0ba-105">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="6e0ba-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ba-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e0ba-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e0ba-107">Properties</span></span>
|<span data-ttu-id="6e0ba-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e0ba-108">Property</span></span>|<span data-ttu-id="6e0ba-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e0ba-109">Type</span></span>|<span data-ttu-id="6e0ba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0ba-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6e0ba-111">displayName</span></span>|<span data-ttu-id="6e0ba-112">String</span><span class="sxs-lookup"><span data-stu-id="6e0ba-112">String</span></span>|<span data-ttu-id="6e0ba-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-113">Display Name.</span></span> <span data-ttu-id="6e0ba-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ba-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6e0ba-115">descrição</span><span class="sxs-lookup"><span data-stu-id="6e0ba-115">description</span></span>|<span data-ttu-id="6e0ba-116">String</span><span class="sxs-lookup"><span data-stu-id="6e0ba-116">String</span></span>|<span data-ttu-id="6e0ba-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-117">Description.</span></span> <span data-ttu-id="6e0ba-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ba-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6e0ba-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="6e0ba-119">omaUri</span></span>|<span data-ttu-id="6e0ba-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e0ba-120">String</span></span>|<span data-ttu-id="6e0ba-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-121">OMA.</span></span> <span data-ttu-id="6e0ba-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ba-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6e0ba-123">value</span><span class="sxs-lookup"><span data-stu-id="6e0ba-123">value</span></span>|<span data-ttu-id="6e0ba-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ba-124">Boolean</span></span>|<span data-ttu-id="6e0ba-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e0ba-126">Relações</span><span class="sxs-lookup"><span data-stu-id="6e0ba-126">Relationships</span></span>
<span data-ttu-id="6e0ba-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e0ba-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e0ba-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e0ba-128">JSON Representation</span></span>
<span data-ttu-id="6e0ba-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e0ba-129">Here is a JSON representation of the resource.</span></span>
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



