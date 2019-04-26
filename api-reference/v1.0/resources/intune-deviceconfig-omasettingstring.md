---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569050"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="feac7-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="feac7-103">omaSettingString resource type</span></span>

> <span data-ttu-id="feac7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="feac7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feac7-105">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="feac7-105">OMA Settings String definition.</span></span>


<span data-ttu-id="feac7-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="feac7-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="feac7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feac7-107">Properties</span></span>
|<span data-ttu-id="feac7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feac7-108">Property</span></span>|<span data-ttu-id="feac7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="feac7-109">Type</span></span>|<span data-ttu-id="feac7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="feac7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feac7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="feac7-111">displayName</span></span>|<span data-ttu-id="feac7-112">String</span><span class="sxs-lookup"><span data-stu-id="feac7-112">String</span></span>|<span data-ttu-id="feac7-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="feac7-113">Display Name.</span></span> <span data-ttu-id="feac7-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="feac7-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="feac7-115">description</span><span class="sxs-lookup"><span data-stu-id="feac7-115">description</span></span>|<span data-ttu-id="feac7-116">String</span><span class="sxs-lookup"><span data-stu-id="feac7-116">String</span></span>|<span data-ttu-id="feac7-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="feac7-117">Description.</span></span> <span data-ttu-id="feac7-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="feac7-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="feac7-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="feac7-119">omaUri</span></span>|<span data-ttu-id="feac7-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feac7-120">String</span></span>|<span data-ttu-id="feac7-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="feac7-121">OMA.</span></span> <span data-ttu-id="feac7-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="feac7-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="feac7-123">value</span><span class="sxs-lookup"><span data-stu-id="feac7-123">value</span></span>|<span data-ttu-id="feac7-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feac7-124">String</span></span>|<span data-ttu-id="feac7-125">Valor.</span><span class="sxs-lookup"><span data-stu-id="feac7-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="feac7-126">Relações</span><span class="sxs-lookup"><span data-stu-id="feac7-126">Relationships</span></span>
<span data-ttu-id="feac7-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feac7-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="feac7-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feac7-128">JSON Representation</span></span>
<span data-ttu-id="feac7-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feac7-129">Here is a JSON representation of the resource.</span></span>
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



