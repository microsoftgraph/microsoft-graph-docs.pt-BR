---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f5885a81e68dbea4e5f6f1c8cae456144785338
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413917"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e7796-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="e7796-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="e7796-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7796-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7796-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7796-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7796-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e7796-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7796-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e7796-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e7796-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e7796-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e7796-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7796-109">Properties</span></span>
|<span data-ttu-id="e7796-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7796-110">Property</span></span>|<span data-ttu-id="e7796-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7796-111">Type</span></span>|<span data-ttu-id="e7796-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7796-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7796-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e7796-113">displayName</span></span>|<span data-ttu-id="e7796-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7796-114">String</span></span>|<span data-ttu-id="e7796-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e7796-115">Display Name.</span></span> <span data-ttu-id="e7796-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e7796-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e7796-117">descrição</span><span class="sxs-lookup"><span data-stu-id="e7796-117">description</span></span>|<span data-ttu-id="e7796-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7796-118">String</span></span>|<span data-ttu-id="e7796-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e7796-119">Description.</span></span> <span data-ttu-id="e7796-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e7796-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e7796-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="e7796-121">omaUri</span></span>|<span data-ttu-id="e7796-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7796-122">String</span></span>|<span data-ttu-id="e7796-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="e7796-123">OMA.</span></span> <span data-ttu-id="e7796-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e7796-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e7796-125">fileName</span><span class="sxs-lookup"><span data-stu-id="e7796-125">fileName</span></span>|<span data-ttu-id="e7796-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7796-126">String</span></span>|<span data-ttu-id="e7796-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="e7796-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e7796-128">CRT</span><span class="sxs-lookup"><span data-stu-id="e7796-128">\*.crt</span></span> | <span data-ttu-id="e7796-129">p7b</span><span class="sxs-lookup"><span data-stu-id="e7796-129">\*.p7b</span></span> | <span data-ttu-id="e7796-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="e7796-130">\*.bin).</span></span>|
|<span data-ttu-id="e7796-131">valor</span><span class="sxs-lookup"><span data-stu-id="e7796-131">value</span></span>|<span data-ttu-id="e7796-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7796-132">String</span></span>|<span data-ttu-id="e7796-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="e7796-133">Value.</span></span> <span data-ttu-id="e7796-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="e7796-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7796-135">Relações</span><span class="sxs-lookup"><span data-stu-id="e7796-135">Relationships</span></span>
<span data-ttu-id="e7796-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7796-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7796-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7796-137">JSON Representation</span></span>
<span data-ttu-id="e7796-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7796-138">Here is a JSON representation of the resource.</span></span>
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




