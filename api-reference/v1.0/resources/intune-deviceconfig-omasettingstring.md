---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30802cc391958fabec4540fc3256f7c67ec094c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031301"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="18c67-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="18c67-103">omaSettingString resource type</span></span>

> <span data-ttu-id="18c67-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18c67-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18c67-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="18c67-105">OMA Settings String definition.</span></span>


<span data-ttu-id="18c67-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="18c67-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18c67-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18c67-107">Properties</span></span>
|<span data-ttu-id="18c67-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18c67-108">Property</span></span>|<span data-ttu-id="18c67-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="18c67-109">Type</span></span>|<span data-ttu-id="18c67-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18c67-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18c67-111">displayName</span><span class="sxs-lookup"><span data-stu-id="18c67-111">displayName</span></span>|<span data-ttu-id="18c67-112">String</span><span class="sxs-lookup"><span data-stu-id="18c67-112">String</span></span>|<span data-ttu-id="18c67-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="18c67-113">Display Name.</span></span> <span data-ttu-id="18c67-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="18c67-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="18c67-115">descrição</span><span class="sxs-lookup"><span data-stu-id="18c67-115">description</span></span>|<span data-ttu-id="18c67-116">String</span><span class="sxs-lookup"><span data-stu-id="18c67-116">String</span></span>|<span data-ttu-id="18c67-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="18c67-117">Description.</span></span> <span data-ttu-id="18c67-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="18c67-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="18c67-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="18c67-119">omaUri</span></span>|<span data-ttu-id="18c67-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18c67-120">String</span></span>|<span data-ttu-id="18c67-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="18c67-121">OMA.</span></span> <span data-ttu-id="18c67-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="18c67-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="18c67-123">value</span><span class="sxs-lookup"><span data-stu-id="18c67-123">value</span></span>|<span data-ttu-id="18c67-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18c67-124">String</span></span>|<span data-ttu-id="18c67-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="18c67-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18c67-126">Relações</span><span class="sxs-lookup"><span data-stu-id="18c67-126">Relationships</span></span>
<span data-ttu-id="18c67-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18c67-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18c67-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18c67-128">JSON Representation</span></span>
<span data-ttu-id="18c67-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18c67-129">Here is a JSON representation of the resource.</span></span>
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



