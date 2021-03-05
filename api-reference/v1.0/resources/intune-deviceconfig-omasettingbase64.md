---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6288803dd87afa7fe45525c20258bdded34482ea
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470750"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="47c93-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="47c93-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="47c93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47c93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47c93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c93-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="47c93-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="47c93-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47c93-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47c93-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47c93-108">Properties</span></span>
|<span data-ttu-id="47c93-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47c93-109">Property</span></span>|<span data-ttu-id="47c93-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="47c93-110">Type</span></span>|<span data-ttu-id="47c93-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47c93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47c93-112">displayName</span><span class="sxs-lookup"><span data-stu-id="47c93-112">displayName</span></span>|<span data-ttu-id="47c93-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c93-113">String</span></span>|<span data-ttu-id="47c93-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="47c93-114">Display Name.</span></span> <span data-ttu-id="47c93-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47c93-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47c93-116">description</span><span class="sxs-lookup"><span data-stu-id="47c93-116">description</span></span>|<span data-ttu-id="47c93-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c93-117">String</span></span>|<span data-ttu-id="47c93-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="47c93-118">Description.</span></span> <span data-ttu-id="47c93-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47c93-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47c93-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="47c93-120">omaUri</span></span>|<span data-ttu-id="47c93-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c93-121">String</span></span>|<span data-ttu-id="47c93-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="47c93-122">OMA.</span></span> <span data-ttu-id="47c93-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47c93-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47c93-124">fileName</span><span class="sxs-lookup"><span data-stu-id="47c93-124">fileName</span></span>|<span data-ttu-id="47c93-125">String</span><span class="sxs-lookup"><span data-stu-id="47c93-125">String</span></span>|<span data-ttu-id="47c93-126">Nome do arquivo associado à propriedade Value (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span><span class="sxs-lookup"><span data-stu-id="47c93-126">File name associated with the Value property (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span></span>|
|<span data-ttu-id="47c93-127">value</span><span class="sxs-lookup"><span data-stu-id="47c93-127">value</span></span>|<span data-ttu-id="47c93-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c93-128">String</span></span>|<span data-ttu-id="47c93-129">Valor.</span><span class="sxs-lookup"><span data-stu-id="47c93-129">Value.</span></span> <span data-ttu-id="47c93-130">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="47c93-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="47c93-131">Relações</span><span class="sxs-lookup"><span data-stu-id="47c93-131">Relationships</span></span>
<span data-ttu-id="47c93-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47c93-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47c93-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47c93-133">JSON Representation</span></span>
<span data-ttu-id="47c93-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47c93-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```









