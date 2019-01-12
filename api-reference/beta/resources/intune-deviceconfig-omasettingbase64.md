---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f1c6a488adf2f39b2c415e31c4919380ebda5ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982565"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="d9de9-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="d9de9-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="d9de9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9de9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9de9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9de9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9de9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d9de9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9de9-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="d9de9-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="d9de9-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d9de9-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9de9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9de9-109">Properties</span></span>
|<span data-ttu-id="d9de9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9de9-110">Property</span></span>|<span data-ttu-id="d9de9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9de9-111">Type</span></span>|<span data-ttu-id="d9de9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9de9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9de9-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d9de9-113">displayName</span></span>|<span data-ttu-id="d9de9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9de9-114">String</span></span>|<span data-ttu-id="d9de9-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d9de9-115">Display Name.</span></span> <span data-ttu-id="d9de9-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d9de9-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d9de9-117">descrição</span><span class="sxs-lookup"><span data-stu-id="d9de9-117">description</span></span>|<span data-ttu-id="d9de9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9de9-118">String</span></span>|<span data-ttu-id="d9de9-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d9de9-119">Description.</span></span> <span data-ttu-id="d9de9-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d9de9-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d9de9-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="d9de9-121">omaUri</span></span>|<span data-ttu-id="d9de9-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9de9-122">String</span></span>|<span data-ttu-id="d9de9-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="d9de9-123">OMA.</span></span> <span data-ttu-id="d9de9-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d9de9-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d9de9-125">fileName</span><span class="sxs-lookup"><span data-stu-id="d9de9-125">fileName</span></span>|<span data-ttu-id="d9de9-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9de9-126">String</span></span>|<span data-ttu-id="d9de9-127">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="d9de9-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="d9de9-128">CRT</span><span class="sxs-lookup"><span data-stu-id="d9de9-128">\*.crt</span></span> | <span data-ttu-id="d9de9-129">p7b</span><span class="sxs-lookup"><span data-stu-id="d9de9-129">\*.p7b</span></span> | <span data-ttu-id="d9de9-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="d9de9-130">\*.bin).</span></span>|
|<span data-ttu-id="d9de9-131">valor</span><span class="sxs-lookup"><span data-stu-id="d9de9-131">value</span></span>|<span data-ttu-id="d9de9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9de9-132">String</span></span>|<span data-ttu-id="d9de9-133">Valor.</span><span class="sxs-lookup"><span data-stu-id="d9de9-133">Value.</span></span> <span data-ttu-id="d9de9-134">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="d9de9-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9de9-135">Relações</span><span class="sxs-lookup"><span data-stu-id="d9de9-135">Relationships</span></span>
<span data-ttu-id="d9de9-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9de9-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9de9-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9de9-137">JSON Representation</span></span>
<span data-ttu-id="d9de9-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9de9-138">Here is a JSON representation of the resource.</span></span>
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





