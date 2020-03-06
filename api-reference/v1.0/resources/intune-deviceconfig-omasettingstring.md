---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 885f2c275cea1df033a3cdfe791297d6b5d70c4c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530570"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="3d247-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="3d247-103">omaSettingString resource type</span></span>

<span data-ttu-id="3d247-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d247-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d247-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d247-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d247-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="3d247-106">OMA Settings String definition.</span></span>


<span data-ttu-id="3d247-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3d247-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d247-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d247-108">Properties</span></span>
|<span data-ttu-id="3d247-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d247-109">Property</span></span>|<span data-ttu-id="3d247-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d247-110">Type</span></span>|<span data-ttu-id="3d247-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d247-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d247-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3d247-112">displayName</span></span>|<span data-ttu-id="3d247-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d247-113">String</span></span>|<span data-ttu-id="3d247-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3d247-114">Display Name.</span></span> <span data-ttu-id="3d247-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3d247-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3d247-116">description</span><span class="sxs-lookup"><span data-stu-id="3d247-116">description</span></span>|<span data-ttu-id="3d247-117">String</span><span class="sxs-lookup"><span data-stu-id="3d247-117">String</span></span>|<span data-ttu-id="3d247-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3d247-118">Description.</span></span> <span data-ttu-id="3d247-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3d247-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3d247-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3d247-120">omaUri</span></span>|<span data-ttu-id="3d247-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d247-121">String</span></span>|<span data-ttu-id="3d247-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="3d247-122">OMA.</span></span> <span data-ttu-id="3d247-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3d247-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3d247-124">value</span><span class="sxs-lookup"><span data-stu-id="3d247-124">value</span></span>|<span data-ttu-id="3d247-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d247-125">String</span></span>|<span data-ttu-id="3d247-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="3d247-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d247-127">Relações</span><span class="sxs-lookup"><span data-stu-id="3d247-127">Relationships</span></span>
<span data-ttu-id="3d247-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d247-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d247-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d247-129">JSON Representation</span></span>
<span data-ttu-id="3d247-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d247-130">Here is a JSON representation of the resource.</span></span>
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




