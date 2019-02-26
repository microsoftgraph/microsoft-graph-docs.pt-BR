---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f95201a725969fa125cdf949874686b9155fc3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252424"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="70671-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="70671-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="70671-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70671-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70671-105">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="70671-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="70671-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="70671-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70671-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70671-107">Properties</span></span>
|<span data-ttu-id="70671-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70671-108">Property</span></span>|<span data-ttu-id="70671-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="70671-109">Type</span></span>|<span data-ttu-id="70671-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="70671-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70671-111">displayName</span><span class="sxs-lookup"><span data-stu-id="70671-111">displayName</span></span>|<span data-ttu-id="70671-112">String</span><span class="sxs-lookup"><span data-stu-id="70671-112">String</span></span>|<span data-ttu-id="70671-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="70671-113">Display Name.</span></span> <span data-ttu-id="70671-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="70671-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="70671-115">descrição</span><span class="sxs-lookup"><span data-stu-id="70671-115">description</span></span>|<span data-ttu-id="70671-116">String</span><span class="sxs-lookup"><span data-stu-id="70671-116">String</span></span>|<span data-ttu-id="70671-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="70671-117">Description.</span></span> <span data-ttu-id="70671-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="70671-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="70671-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="70671-119">omaUri</span></span>|<span data-ttu-id="70671-120">String</span><span class="sxs-lookup"><span data-stu-id="70671-120">String</span></span>|<span data-ttu-id="70671-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="70671-121">OMA.</span></span> <span data-ttu-id="70671-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="70671-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="70671-123">fileName</span><span class="sxs-lookup"><span data-stu-id="70671-123">fileName</span></span>|<span data-ttu-id="70671-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70671-124">String</span></span>|<span data-ttu-id="70671-125">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="70671-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="70671-126">valor</span><span class="sxs-lookup"><span data-stu-id="70671-126">value</span></span>|<span data-ttu-id="70671-127">Binário</span><span class="sxs-lookup"><span data-stu-id="70671-127">Binary</span></span>|<span data-ttu-id="70671-128">Valor.</span><span class="sxs-lookup"><span data-stu-id="70671-128">Value.</span></span> <span data-ttu-id="70671-129">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="70671-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="70671-130">Relações</span><span class="sxs-lookup"><span data-stu-id="70671-130">Relationships</span></span>
<span data-ttu-id="70671-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70671-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70671-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70671-132">JSON Representation</span></span>
<span data-ttu-id="70671-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70671-133">Here is a JSON representation of the resource.</span></span>
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



