---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b33dde8c6d24432d1eb5b4823873a9da712faf7d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529548"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="0f480-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="0f480-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="0f480-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0f480-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f480-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f480-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f480-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f480-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f480-107">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="0f480-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="0f480-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f480-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f480-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f480-109">Properties</span></span>
|<span data-ttu-id="0f480-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f480-110">Property</span></span>|<span data-ttu-id="0f480-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f480-111">Type</span></span>|<span data-ttu-id="0f480-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f480-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f480-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0f480-113">displayName</span></span>|<span data-ttu-id="0f480-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f480-114">String</span></span>|<span data-ttu-id="0f480-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="0f480-115">Display Name.</span></span> <span data-ttu-id="0f480-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f480-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f480-117">description</span><span class="sxs-lookup"><span data-stu-id="0f480-117">description</span></span>|<span data-ttu-id="0f480-118">String</span><span class="sxs-lookup"><span data-stu-id="0f480-118">String</span></span>|<span data-ttu-id="0f480-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="0f480-119">Description.</span></span> <span data-ttu-id="0f480-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f480-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f480-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="0f480-121">omaUri</span></span>|<span data-ttu-id="0f480-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f480-122">String</span></span>|<span data-ttu-id="0f480-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="0f480-123">OMA.</span></span> <span data-ttu-id="0f480-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f480-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f480-125">fileName</span><span class="sxs-lookup"><span data-stu-id="0f480-125">fileName</span></span>|<span data-ttu-id="0f480-126">String</span><span class="sxs-lookup"><span data-stu-id="0f480-126">String</span></span>|<span data-ttu-id="0f480-127">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="0f480-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="0f480-128">valor</span><span class="sxs-lookup"><span data-stu-id="0f480-128">value</span></span>|<span data-ttu-id="0f480-129">Binário</span><span class="sxs-lookup"><span data-stu-id="0f480-129">Binary</span></span>|<span data-ttu-id="0f480-130">Valor.</span><span class="sxs-lookup"><span data-stu-id="0f480-130">Value.</span></span> <span data-ttu-id="0f480-131">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="0f480-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f480-132">Relações</span><span class="sxs-lookup"><span data-stu-id="0f480-132">Relationships</span></span>
<span data-ttu-id="0f480-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f480-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f480-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f480-134">JSON Representation</span></span>
<span data-ttu-id="0f480-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f480-135">Here is a JSON representation of the resource.</span></span>
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



