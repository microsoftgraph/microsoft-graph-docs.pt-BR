---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33488e3b6500056c0f183d5e219e5f5ec489c178
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534875"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="3529f-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="3529f-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="3529f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3529f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3529f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3529f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3529f-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="3529f-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="3529f-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3529f-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3529f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3529f-108">Properties</span></span>
|<span data-ttu-id="3529f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3529f-109">Property</span></span>|<span data-ttu-id="3529f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3529f-110">Type</span></span>|<span data-ttu-id="3529f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3529f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3529f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3529f-112">displayName</span></span>|<span data-ttu-id="3529f-113">String</span><span class="sxs-lookup"><span data-stu-id="3529f-113">String</span></span>|<span data-ttu-id="3529f-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3529f-114">Display Name.</span></span> <span data-ttu-id="3529f-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3529f-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3529f-116">description</span><span class="sxs-lookup"><span data-stu-id="3529f-116">description</span></span>|<span data-ttu-id="3529f-117">String</span><span class="sxs-lookup"><span data-stu-id="3529f-117">String</span></span>|<span data-ttu-id="3529f-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3529f-118">Description.</span></span> <span data-ttu-id="3529f-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3529f-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3529f-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3529f-120">omaUri</span></span>|<span data-ttu-id="3529f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3529f-121">String</span></span>|<span data-ttu-id="3529f-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="3529f-122">OMA.</span></span> <span data-ttu-id="3529f-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3529f-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3529f-124">fileName</span><span class="sxs-lookup"><span data-stu-id="3529f-124">fileName</span></span>|<span data-ttu-id="3529f-125">String</span><span class="sxs-lookup"><span data-stu-id="3529f-125">String</span></span>|<span data-ttu-id="3529f-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="3529f-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="3529f-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="3529f-127">\*.crt</span></span> | <span data-ttu-id="3529f-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="3529f-128">\*.p7b</span></span> | <span data-ttu-id="3529f-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="3529f-129">\*.bin).</span></span>|
|<span data-ttu-id="3529f-130">value</span><span class="sxs-lookup"><span data-stu-id="3529f-130">value</span></span>|<span data-ttu-id="3529f-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3529f-131">String</span></span>|<span data-ttu-id="3529f-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="3529f-132">Value.</span></span> <span data-ttu-id="3529f-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="3529f-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3529f-134">Relações</span><span class="sxs-lookup"><span data-stu-id="3529f-134">Relationships</span></span>
<span data-ttu-id="3529f-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3529f-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3529f-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3529f-136">JSON Representation</span></span>
<span data-ttu-id="3529f-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3529f-137">Here is a JSON representation of the resource.</span></span>
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





