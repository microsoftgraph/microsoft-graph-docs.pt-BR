---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ddce8acb059ff28ad37bce284efc6f3fd29f0224
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368440"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="edbf2-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="edbf2-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="edbf2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edbf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edbf2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edbf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edbf2-106">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="edbf2-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="edbf2-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="edbf2-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="edbf2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edbf2-108">Properties</span></span>
|<span data-ttu-id="edbf2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edbf2-109">Property</span></span>|<span data-ttu-id="edbf2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="edbf2-110">Type</span></span>|<span data-ttu-id="edbf2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbf2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="edbf2-112">displayName</span></span>|<span data-ttu-id="edbf2-113">String</span><span class="sxs-lookup"><span data-stu-id="edbf2-113">String</span></span>|<span data-ttu-id="edbf2-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="edbf2-114">Display Name.</span></span> <span data-ttu-id="edbf2-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="edbf2-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="edbf2-116">descrição</span><span class="sxs-lookup"><span data-stu-id="edbf2-116">description</span></span>|<span data-ttu-id="edbf2-117">String</span><span class="sxs-lookup"><span data-stu-id="edbf2-117">String</span></span>|<span data-ttu-id="edbf2-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="edbf2-118">Description.</span></span> <span data-ttu-id="edbf2-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="edbf2-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="edbf2-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="edbf2-120">omaUri</span></span>|<span data-ttu-id="edbf2-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbf2-121">String</span></span>|<span data-ttu-id="edbf2-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="edbf2-122">OMA.</span></span> <span data-ttu-id="edbf2-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="edbf2-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="edbf2-124">fileName</span><span class="sxs-lookup"><span data-stu-id="edbf2-124">fileName</span></span>|<span data-ttu-id="edbf2-125">String</span><span class="sxs-lookup"><span data-stu-id="edbf2-125">String</span></span>|<span data-ttu-id="edbf2-126">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="edbf2-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="edbf2-127">valor</span><span class="sxs-lookup"><span data-stu-id="edbf2-127">value</span></span>|<span data-ttu-id="edbf2-128">Binário</span><span class="sxs-lookup"><span data-stu-id="edbf2-128">Binary</span></span>|<span data-ttu-id="edbf2-129">Valor.</span><span class="sxs-lookup"><span data-stu-id="edbf2-129">Value.</span></span> <span data-ttu-id="edbf2-130">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="edbf2-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="edbf2-131">Relações</span><span class="sxs-lookup"><span data-stu-id="edbf2-131">Relationships</span></span>
<span data-ttu-id="edbf2-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="edbf2-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edbf2-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edbf2-133">JSON Representation</span></span>
<span data-ttu-id="edbf2-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edbf2-134">Here is a JSON representation of the resource.</span></span>
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



