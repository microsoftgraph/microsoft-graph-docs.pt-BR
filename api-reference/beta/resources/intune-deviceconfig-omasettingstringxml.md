---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 846ed1c9bb17065b82f2663e7f4276b34442f9bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164530"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="e2598-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="e2598-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="e2598-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2598-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2598-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2598-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2598-106">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e2598-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="e2598-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2598-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2598-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2598-108">Properties</span></span>
|<span data-ttu-id="e2598-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2598-109">Property</span></span>|<span data-ttu-id="e2598-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2598-110">Type</span></span>|<span data-ttu-id="e2598-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2598-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2598-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e2598-112">displayName</span></span>|<span data-ttu-id="e2598-113">String</span><span class="sxs-lookup"><span data-stu-id="e2598-113">String</span></span>|<span data-ttu-id="e2598-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e2598-114">Display Name.</span></span> <span data-ttu-id="e2598-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2598-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2598-116">descrição</span><span class="sxs-lookup"><span data-stu-id="e2598-116">description</span></span>|<span data-ttu-id="e2598-117">String</span><span class="sxs-lookup"><span data-stu-id="e2598-117">String</span></span>|<span data-ttu-id="e2598-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e2598-118">Description.</span></span> <span data-ttu-id="e2598-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2598-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2598-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="e2598-120">omaUri</span></span>|<span data-ttu-id="e2598-121">String</span><span class="sxs-lookup"><span data-stu-id="e2598-121">String</span></span>|<span data-ttu-id="e2598-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="e2598-122">OMA.</span></span> <span data-ttu-id="e2598-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2598-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2598-124">fileName</span><span class="sxs-lookup"><span data-stu-id="e2598-124">fileName</span></span>|<span data-ttu-id="e2598-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2598-125">String</span></span>|<span data-ttu-id="e2598-126">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="e2598-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="e2598-127">valor</span><span class="sxs-lookup"><span data-stu-id="e2598-127">value</span></span>|<span data-ttu-id="e2598-128">Binário</span><span class="sxs-lookup"><span data-stu-id="e2598-128">Binary</span></span>|<span data-ttu-id="e2598-129">Valor.</span><span class="sxs-lookup"><span data-stu-id="e2598-129">Value.</span></span> <span data-ttu-id="e2598-130">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="e2598-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2598-131">Relações</span><span class="sxs-lookup"><span data-stu-id="e2598-131">Relationships</span></span>
<span data-ttu-id="e2598-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2598-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2598-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2598-133">JSON Representation</span></span>
<span data-ttu-id="e2598-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2598-134">Here is a JSON representation of the resource.</span></span>
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




