---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549378"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="1aee6-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="1aee6-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="1aee6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1aee6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aee6-105">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1aee6-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="1aee6-106">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1aee6-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1aee6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1aee6-107">Properties</span></span>
|<span data-ttu-id="1aee6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aee6-108">Property</span></span>|<span data-ttu-id="1aee6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aee6-109">Type</span></span>|<span data-ttu-id="1aee6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aee6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aee6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1aee6-111">displayName</span></span>|<span data-ttu-id="1aee6-112">String</span><span class="sxs-lookup"><span data-stu-id="1aee6-112">String</span></span>|<span data-ttu-id="1aee6-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1aee6-113">Display Name.</span></span> <span data-ttu-id="1aee6-114">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1aee6-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1aee6-115">description</span><span class="sxs-lookup"><span data-stu-id="1aee6-115">description</span></span>|<span data-ttu-id="1aee6-116">String</span><span class="sxs-lookup"><span data-stu-id="1aee6-116">String</span></span>|<span data-ttu-id="1aee6-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1aee6-117">Description.</span></span> <span data-ttu-id="1aee6-118">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1aee6-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1aee6-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="1aee6-119">omaUri</span></span>|<span data-ttu-id="1aee6-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1aee6-120">String</span></span>|<span data-ttu-id="1aee6-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="1aee6-121">OMA.</span></span> <span data-ttu-id="1aee6-122">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1aee6-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1aee6-123">fileName</span><span class="sxs-lookup"><span data-stu-id="1aee6-123">fileName</span></span>|<span data-ttu-id="1aee6-124">String</span><span class="sxs-lookup"><span data-stu-id="1aee6-124">String</span></span>|<span data-ttu-id="1aee6-125">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="1aee6-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="1aee6-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="1aee6-126">\*.crt</span></span> | <span data-ttu-id="1aee6-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="1aee6-127">\*.p7b</span></span> | <span data-ttu-id="1aee6-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="1aee6-128">\*.bin).</span></span>|
|<span data-ttu-id="1aee6-129">value</span><span class="sxs-lookup"><span data-stu-id="1aee6-129">value</span></span>|<span data-ttu-id="1aee6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1aee6-130">String</span></span>|<span data-ttu-id="1aee6-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="1aee6-131">Value.</span></span> <span data-ttu-id="1aee6-132">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="1aee6-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aee6-133">Relações</span><span class="sxs-lookup"><span data-stu-id="1aee6-133">Relationships</span></span>
<span data-ttu-id="1aee6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1aee6-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aee6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1aee6-135">JSON Representation</span></span>
<span data-ttu-id="1aee6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1aee6-136">Here is a JSON representation of the resource.</span></span>
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



