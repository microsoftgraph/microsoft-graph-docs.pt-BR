---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
ms.openlocfilehash: ecdc22f698479ba25a2cce4ce822cda633c582ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003560"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="873f5-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="873f5-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="873f5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="873f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="873f5-105">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="873f5-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="873f5-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="873f5-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="873f5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="873f5-107">Properties</span></span>
|<span data-ttu-id="873f5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="873f5-108">Property</span></span>|<span data-ttu-id="873f5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="873f5-109">Type</span></span>|<span data-ttu-id="873f5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="873f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="873f5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="873f5-111">displayName</span></span>|<span data-ttu-id="873f5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="873f5-112">String</span></span>|<span data-ttu-id="873f5-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="873f5-113">Display Name.</span></span> <span data-ttu-id="873f5-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="873f5-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="873f5-115">descrição</span><span class="sxs-lookup"><span data-stu-id="873f5-115">description</span></span>|<span data-ttu-id="873f5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="873f5-116">String</span></span>|<span data-ttu-id="873f5-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="873f5-117">Description.</span></span> <span data-ttu-id="873f5-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="873f5-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="873f5-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="873f5-119">omaUri</span></span>|<span data-ttu-id="873f5-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="873f5-120">String</span></span>|<span data-ttu-id="873f5-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="873f5-121">OMA.</span></span> <span data-ttu-id="873f5-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="873f5-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="873f5-123">fileName</span><span class="sxs-lookup"><span data-stu-id="873f5-123">fileName</span></span>|<span data-ttu-id="873f5-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="873f5-124">String</span></span>|<span data-ttu-id="873f5-125">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="873f5-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="873f5-126">valor</span><span class="sxs-lookup"><span data-stu-id="873f5-126">value</span></span>|<span data-ttu-id="873f5-127">Binário</span><span class="sxs-lookup"><span data-stu-id="873f5-127">Binary</span></span>|<span data-ttu-id="873f5-128">Valor.</span><span class="sxs-lookup"><span data-stu-id="873f5-128">Value.</span></span> <span data-ttu-id="873f5-129">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="873f5-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="873f5-130">Relações</span><span class="sxs-lookup"><span data-stu-id="873f5-130">Relationships</span></span>
<span data-ttu-id="873f5-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="873f5-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="873f5-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="873f5-132">JSON Representation</span></span>
<span data-ttu-id="873f5-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="873f5-133">Here is a JSON representation of the resource.</span></span>
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



