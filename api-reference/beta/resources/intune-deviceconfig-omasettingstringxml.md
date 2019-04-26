---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8dbc23845f62c5f2a70af9051efa732b3d3d8ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566742"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="19b53-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="19b53-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="19b53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19b53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19b53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19b53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b53-106">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="19b53-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="19b53-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19b53-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19b53-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19b53-108">Properties</span></span>
|<span data-ttu-id="19b53-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19b53-109">Property</span></span>|<span data-ttu-id="19b53-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b53-110">Type</span></span>|<span data-ttu-id="19b53-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b53-112">displayName</span><span class="sxs-lookup"><span data-stu-id="19b53-112">displayName</span></span>|<span data-ttu-id="19b53-113">String</span><span class="sxs-lookup"><span data-stu-id="19b53-113">String</span></span>|<span data-ttu-id="19b53-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="19b53-114">Display Name.</span></span> <span data-ttu-id="19b53-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19b53-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="19b53-116">description</span><span class="sxs-lookup"><span data-stu-id="19b53-116">description</span></span>|<span data-ttu-id="19b53-117">String</span><span class="sxs-lookup"><span data-stu-id="19b53-117">String</span></span>|<span data-ttu-id="19b53-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="19b53-118">Description.</span></span> <span data-ttu-id="19b53-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19b53-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="19b53-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="19b53-120">omaUri</span></span>|<span data-ttu-id="19b53-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19b53-121">String</span></span>|<span data-ttu-id="19b53-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="19b53-122">OMA.</span></span> <span data-ttu-id="19b53-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19b53-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="19b53-124">fileName</span><span class="sxs-lookup"><span data-stu-id="19b53-124">fileName</span></span>|<span data-ttu-id="19b53-125">String</span><span class="sxs-lookup"><span data-stu-id="19b53-125">String</span></span>|<span data-ttu-id="19b53-126">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="19b53-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="19b53-127">valor</span><span class="sxs-lookup"><span data-stu-id="19b53-127">value</span></span>|<span data-ttu-id="19b53-128">Binário</span><span class="sxs-lookup"><span data-stu-id="19b53-128">Binary</span></span>|<span data-ttu-id="19b53-129">Valor.</span><span class="sxs-lookup"><span data-stu-id="19b53-129">Value.</span></span> <span data-ttu-id="19b53-130">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="19b53-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="19b53-131">Relações</span><span class="sxs-lookup"><span data-stu-id="19b53-131">Relationships</span></span>
<span data-ttu-id="19b53-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19b53-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19b53-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19b53-133">JSON Representation</span></span>
<span data-ttu-id="19b53-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19b53-134">Here is a JSON representation of the resource.</span></span>
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





