---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 976c95ed9ffa6674ddc185bb1723c7d7f9d054f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894016"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="b8c15-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="b8c15-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="b8c15-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8c15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8c15-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8c15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8c15-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b8c15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8c15-107">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b8c15-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="b8c15-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b8c15-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8c15-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8c15-109">Properties</span></span>
|<span data-ttu-id="b8c15-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8c15-110">Property</span></span>|<span data-ttu-id="b8c15-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8c15-111">Type</span></span>|<span data-ttu-id="b8c15-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8c15-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8c15-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b8c15-113">displayName</span></span>|<span data-ttu-id="b8c15-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c15-114">String</span></span>|<span data-ttu-id="b8c15-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b8c15-115">Display Name.</span></span> <span data-ttu-id="b8c15-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b8c15-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b8c15-117">descrição</span><span class="sxs-lookup"><span data-stu-id="b8c15-117">description</span></span>|<span data-ttu-id="b8c15-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c15-118">String</span></span>|<span data-ttu-id="b8c15-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b8c15-119">Description.</span></span> <span data-ttu-id="b8c15-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b8c15-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b8c15-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b8c15-121">omaUri</span></span>|<span data-ttu-id="b8c15-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c15-122">String</span></span>|<span data-ttu-id="b8c15-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="b8c15-123">OMA.</span></span> <span data-ttu-id="b8c15-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b8c15-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b8c15-125">fileName</span><span class="sxs-lookup"><span data-stu-id="b8c15-125">fileName</span></span>|<span data-ttu-id="b8c15-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c15-126">String</span></span>|<span data-ttu-id="b8c15-127">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="b8c15-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="b8c15-128">valor</span><span class="sxs-lookup"><span data-stu-id="b8c15-128">value</span></span>|<span data-ttu-id="b8c15-129">Binário</span><span class="sxs-lookup"><span data-stu-id="b8c15-129">Binary</span></span>|<span data-ttu-id="b8c15-130">Valor.</span><span class="sxs-lookup"><span data-stu-id="b8c15-130">Value.</span></span> <span data-ttu-id="b8c15-131">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="b8c15-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8c15-132">Relações</span><span class="sxs-lookup"><span data-stu-id="b8c15-132">Relationships</span></span>
<span data-ttu-id="b8c15-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8c15-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8c15-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8c15-134">JSON Representation</span></span>
<span data-ttu-id="b8c15-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8c15-135">Here is a JSON representation of the resource.</span></span>
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





