---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37c8996eb59186d8b8d5c0c486d40a7b06ce2dc5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788426"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="245f1-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="245f1-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="245f1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="245f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="245f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="245f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="245f1-106">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="245f1-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="245f1-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="245f1-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="245f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="245f1-108">Properties</span></span>
|<span data-ttu-id="245f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="245f1-109">Property</span></span>|<span data-ttu-id="245f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="245f1-110">Type</span></span>|<span data-ttu-id="245f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="245f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="245f1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="245f1-112">displayName</span></span>|<span data-ttu-id="245f1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="245f1-113">String</span></span>|<span data-ttu-id="245f1-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="245f1-114">Display Name.</span></span> <span data-ttu-id="245f1-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="245f1-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="245f1-116">description</span><span class="sxs-lookup"><span data-stu-id="245f1-116">description</span></span>|<span data-ttu-id="245f1-117">String</span><span class="sxs-lookup"><span data-stu-id="245f1-117">String</span></span>|<span data-ttu-id="245f1-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="245f1-118">Description.</span></span> <span data-ttu-id="245f1-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="245f1-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="245f1-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="245f1-120">omaUri</span></span>|<span data-ttu-id="245f1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="245f1-121">String</span></span>|<span data-ttu-id="245f1-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="245f1-122">OMA.</span></span> <span data-ttu-id="245f1-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="245f1-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="245f1-124">fileName</span><span class="sxs-lookup"><span data-stu-id="245f1-124">fileName</span></span>|<span data-ttu-id="245f1-125">String</span><span class="sxs-lookup"><span data-stu-id="245f1-125">String</span></span>|<span data-ttu-id="245f1-126">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="245f1-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="245f1-127">valor</span><span class="sxs-lookup"><span data-stu-id="245f1-127">value</span></span>|<span data-ttu-id="245f1-128">Binário</span><span class="sxs-lookup"><span data-stu-id="245f1-128">Binary</span></span>|<span data-ttu-id="245f1-129">Valor.</span><span class="sxs-lookup"><span data-stu-id="245f1-129">Value.</span></span> <span data-ttu-id="245f1-130">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="245f1-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="245f1-131">Relações</span><span class="sxs-lookup"><span data-stu-id="245f1-131">Relationships</span></span>
<span data-ttu-id="245f1-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="245f1-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="245f1-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="245f1-133">JSON Representation</span></span>
<span data-ttu-id="245f1-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="245f1-134">Here is a JSON representation of the resource.</span></span>
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



