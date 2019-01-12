---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e34dc1ebdfff2692d35d258492bc58cb26282198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911480"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="f38a4-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="f38a4-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="f38a4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f38a4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f38a4-105">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f38a4-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="f38a4-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f38a4-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f38a4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f38a4-107">Properties</span></span>
|<span data-ttu-id="f38a4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f38a4-108">Property</span></span>|<span data-ttu-id="f38a4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38a4-109">Type</span></span>|<span data-ttu-id="f38a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f38a4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f38a4-111">displayName</span></span>|<span data-ttu-id="f38a4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38a4-112">String</span></span>|<span data-ttu-id="f38a4-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f38a4-113">Display Name.</span></span> <span data-ttu-id="f38a4-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f38a4-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f38a4-115">descrição</span><span class="sxs-lookup"><span data-stu-id="f38a4-115">description</span></span>|<span data-ttu-id="f38a4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38a4-116">String</span></span>|<span data-ttu-id="f38a4-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f38a4-117">Description.</span></span> <span data-ttu-id="f38a4-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f38a4-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f38a4-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f38a4-119">omaUri</span></span>|<span data-ttu-id="f38a4-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38a4-120">String</span></span>|<span data-ttu-id="f38a4-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="f38a4-121">OMA.</span></span> <span data-ttu-id="f38a4-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f38a4-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f38a4-123">fileName</span><span class="sxs-lookup"><span data-stu-id="f38a4-123">fileName</span></span>|<span data-ttu-id="f38a4-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38a4-124">String</span></span>|<span data-ttu-id="f38a4-125">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="f38a4-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="f38a4-126">valor</span><span class="sxs-lookup"><span data-stu-id="f38a4-126">value</span></span>|<span data-ttu-id="f38a4-127">Binário</span><span class="sxs-lookup"><span data-stu-id="f38a4-127">Binary</span></span>|<span data-ttu-id="f38a4-128">Valor.</span><span class="sxs-lookup"><span data-stu-id="f38a4-128">Value.</span></span> <span data-ttu-id="f38a4-129">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="f38a4-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f38a4-130">Relações</span><span class="sxs-lookup"><span data-stu-id="f38a4-130">Relationships</span></span>
<span data-ttu-id="f38a4-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f38a4-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f38a4-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f38a4-132">JSON Representation</span></span>
<span data-ttu-id="f38a4-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f38a4-133">Here is a JSON representation of the resource.</span></span>
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



