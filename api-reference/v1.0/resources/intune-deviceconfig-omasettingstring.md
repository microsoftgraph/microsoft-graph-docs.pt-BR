---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05f37b94aecadd5e3da1d0e162cd8bf6afe96681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988265"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="a9723-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="a9723-103">omaSettingString resource type</span></span>

<span data-ttu-id="a9723-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9723-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9723-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9723-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9723-106">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a9723-106">OMA Settings String definition.</span></span>


<span data-ttu-id="a9723-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9723-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9723-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9723-108">Properties</span></span>
|<span data-ttu-id="a9723-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9723-109">Property</span></span>|<span data-ttu-id="a9723-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9723-110">Type</span></span>|<span data-ttu-id="a9723-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9723-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9723-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a9723-112">displayName</span></span>|<span data-ttu-id="a9723-113">String</span><span class="sxs-lookup"><span data-stu-id="a9723-113">String</span></span>|<span data-ttu-id="a9723-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a9723-114">Display Name.</span></span> <span data-ttu-id="a9723-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9723-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9723-116">description</span><span class="sxs-lookup"><span data-stu-id="a9723-116">description</span></span>|<span data-ttu-id="a9723-117">String</span><span class="sxs-lookup"><span data-stu-id="a9723-117">String</span></span>|<span data-ttu-id="a9723-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a9723-118">Description.</span></span> <span data-ttu-id="a9723-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9723-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9723-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="a9723-120">omaUri</span></span>|<span data-ttu-id="a9723-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9723-121">String</span></span>|<span data-ttu-id="a9723-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="a9723-122">OMA.</span></span> <span data-ttu-id="a9723-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9723-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9723-124">value</span><span class="sxs-lookup"><span data-stu-id="a9723-124">value</span></span>|<span data-ttu-id="a9723-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9723-125">String</span></span>|<span data-ttu-id="a9723-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="a9723-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9723-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a9723-127">Relationships</span></span>
<span data-ttu-id="a9723-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9723-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9723-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9723-129">JSON Representation</span></span>
<span data-ttu-id="a9723-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9723-130">Here is a JSON representation of the resource.</span></span>
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









