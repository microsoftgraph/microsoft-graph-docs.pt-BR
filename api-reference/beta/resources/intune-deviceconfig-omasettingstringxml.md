---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ef4b46f375757419f63f11e0178ed4ab9ea5e11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437070"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="30800-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="30800-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="30800-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30800-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30800-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30800-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30800-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30800-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30800-107">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="30800-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="30800-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="30800-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30800-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30800-109">Properties</span></span>
|<span data-ttu-id="30800-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30800-110">Property</span></span>|<span data-ttu-id="30800-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="30800-111">Type</span></span>|<span data-ttu-id="30800-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="30800-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30800-113">displayName</span><span class="sxs-lookup"><span data-stu-id="30800-113">displayName</span></span>|<span data-ttu-id="30800-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30800-114">String</span></span>|<span data-ttu-id="30800-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="30800-115">Display Name.</span></span> <span data-ttu-id="30800-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="30800-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="30800-117">description</span><span class="sxs-lookup"><span data-stu-id="30800-117">description</span></span>|<span data-ttu-id="30800-118">String</span><span class="sxs-lookup"><span data-stu-id="30800-118">String</span></span>|<span data-ttu-id="30800-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="30800-119">Description.</span></span> <span data-ttu-id="30800-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="30800-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="30800-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="30800-121">omaUri</span></span>|<span data-ttu-id="30800-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30800-122">String</span></span>|<span data-ttu-id="30800-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="30800-123">OMA.</span></span> <span data-ttu-id="30800-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="30800-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="30800-125">fileName</span><span class="sxs-lookup"><span data-stu-id="30800-125">fileName</span></span>|<span data-ttu-id="30800-126">String</span><span class="sxs-lookup"><span data-stu-id="30800-126">String</span></span>|<span data-ttu-id="30800-127">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="30800-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="30800-128">valor</span><span class="sxs-lookup"><span data-stu-id="30800-128">value</span></span>|<span data-ttu-id="30800-129">Binário</span><span class="sxs-lookup"><span data-stu-id="30800-129">Binary</span></span>|<span data-ttu-id="30800-130">Valor.</span><span class="sxs-lookup"><span data-stu-id="30800-130">Value.</span></span> <span data-ttu-id="30800-131">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="30800-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="30800-132">Relações</span><span class="sxs-lookup"><span data-stu-id="30800-132">Relationships</span></span>
<span data-ttu-id="30800-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30800-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30800-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30800-134">JSON Representation</span></span>
<span data-ttu-id="30800-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30800-135">Here is a JSON representation of the resource.</span></span>
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



