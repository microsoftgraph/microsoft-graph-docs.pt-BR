---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 077593048b6dc1aa2611b9e87c506db43fffe922
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359905"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="cb30e-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="cb30e-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="cb30e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb30e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb30e-105">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="cb30e-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="cb30e-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb30e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb30e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb30e-107">Properties</span></span>
|<span data-ttu-id="cb30e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb30e-108">Property</span></span>|<span data-ttu-id="cb30e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb30e-109">Type</span></span>|<span data-ttu-id="cb30e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb30e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb30e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cb30e-111">displayName</span></span>|<span data-ttu-id="cb30e-112">String</span><span class="sxs-lookup"><span data-stu-id="cb30e-112">String</span></span>|<span data-ttu-id="cb30e-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="cb30e-113">Display Name.</span></span> <span data-ttu-id="cb30e-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb30e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb30e-115">descrição</span><span class="sxs-lookup"><span data-stu-id="cb30e-115">description</span></span>|<span data-ttu-id="cb30e-116">String</span><span class="sxs-lookup"><span data-stu-id="cb30e-116">String</span></span>|<span data-ttu-id="cb30e-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="cb30e-117">Description.</span></span> <span data-ttu-id="cb30e-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb30e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb30e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="cb30e-119">omaUri</span></span>|<span data-ttu-id="cb30e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb30e-120">String</span></span>|<span data-ttu-id="cb30e-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="cb30e-121">OMA.</span></span> <span data-ttu-id="cb30e-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb30e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb30e-123">fileName</span><span class="sxs-lookup"><span data-stu-id="cb30e-123">fileName</span></span>|<span data-ttu-id="cb30e-124">String</span><span class="sxs-lookup"><span data-stu-id="cb30e-124">String</span></span>|<span data-ttu-id="cb30e-125">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="cb30e-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="cb30e-126">valor</span><span class="sxs-lookup"><span data-stu-id="cb30e-126">value</span></span>|<span data-ttu-id="cb30e-127">Binário</span><span class="sxs-lookup"><span data-stu-id="cb30e-127">Binary</span></span>|<span data-ttu-id="cb30e-128">Valor.</span><span class="sxs-lookup"><span data-stu-id="cb30e-128">Value.</span></span> <span data-ttu-id="cb30e-129">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="cb30e-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb30e-130">Relações</span><span class="sxs-lookup"><span data-stu-id="cb30e-130">Relationships</span></span>
<span data-ttu-id="cb30e-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb30e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb30e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb30e-132">JSON Representation</span></span>
<span data-ttu-id="cb30e-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb30e-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```




