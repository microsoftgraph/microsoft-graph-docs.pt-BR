---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 177942dd3374b063ecd7b26c657e152643d09288
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722940"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="b1571-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="b1571-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="b1571-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1571-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1571-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1571-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1571-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1571-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1571-107">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b1571-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="b1571-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1571-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b1571-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1571-109">Properties</span></span>
|<span data-ttu-id="b1571-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1571-110">Property</span></span>|<span data-ttu-id="b1571-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1571-111">Type</span></span>|<span data-ttu-id="b1571-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1571-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1571-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b1571-113">displayName</span></span>|<span data-ttu-id="b1571-114">String</span><span class="sxs-lookup"><span data-stu-id="b1571-114">String</span></span>|<span data-ttu-id="b1571-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b1571-115">Display Name.</span></span> <span data-ttu-id="b1571-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1571-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1571-117">description</span><span class="sxs-lookup"><span data-stu-id="b1571-117">description</span></span>|<span data-ttu-id="b1571-118">String</span><span class="sxs-lookup"><span data-stu-id="b1571-118">String</span></span>|<span data-ttu-id="b1571-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b1571-119">Description.</span></span> <span data-ttu-id="b1571-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1571-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1571-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b1571-121">omaUri</span></span>|<span data-ttu-id="b1571-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1571-122">String</span></span>|<span data-ttu-id="b1571-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="b1571-123">OMA.</span></span> <span data-ttu-id="b1571-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1571-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1571-125">fileName</span><span class="sxs-lookup"><span data-stu-id="b1571-125">fileName</span></span>|<span data-ttu-id="b1571-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1571-126">String</span></span>|<span data-ttu-id="b1571-127">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="b1571-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="b1571-128">valor</span><span class="sxs-lookup"><span data-stu-id="b1571-128">value</span></span>|<span data-ttu-id="b1571-129">Binário</span><span class="sxs-lookup"><span data-stu-id="b1571-129">Binary</span></span>|<span data-ttu-id="b1571-130">Valor.</span><span class="sxs-lookup"><span data-stu-id="b1571-130">Value.</span></span> <span data-ttu-id="b1571-131">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="b1571-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1571-132">Relações</span><span class="sxs-lookup"><span data-stu-id="b1571-132">Relationships</span></span>
<span data-ttu-id="b1571-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1571-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1571-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1571-134">JSON Representation</span></span>
<span data-ttu-id="b1571-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1571-135">Here is a JSON representation of the resource.</span></span>
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





