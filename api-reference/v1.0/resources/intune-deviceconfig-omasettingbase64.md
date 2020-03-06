---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9aa6dd320fd04c352208692f988ea487eb28a47c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530595"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="df187-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="df187-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="df187-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df187-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df187-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df187-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df187-106">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="df187-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="df187-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df187-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df187-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df187-108">Properties</span></span>
|<span data-ttu-id="df187-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df187-109">Property</span></span>|<span data-ttu-id="df187-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="df187-110">Type</span></span>|<span data-ttu-id="df187-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df187-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df187-112">displayName</span><span class="sxs-lookup"><span data-stu-id="df187-112">displayName</span></span>|<span data-ttu-id="df187-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df187-113">String</span></span>|<span data-ttu-id="df187-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="df187-114">Display Name.</span></span> <span data-ttu-id="df187-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df187-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="df187-116">description</span><span class="sxs-lookup"><span data-stu-id="df187-116">description</span></span>|<span data-ttu-id="df187-117">String</span><span class="sxs-lookup"><span data-stu-id="df187-117">String</span></span>|<span data-ttu-id="df187-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="df187-118">Description.</span></span> <span data-ttu-id="df187-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df187-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="df187-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="df187-120">omaUri</span></span>|<span data-ttu-id="df187-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df187-121">String</span></span>|<span data-ttu-id="df187-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="df187-122">OMA.</span></span> <span data-ttu-id="df187-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df187-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="df187-124">fileName</span><span class="sxs-lookup"><span data-stu-id="df187-124">fileName</span></span>|<span data-ttu-id="df187-125">String</span><span class="sxs-lookup"><span data-stu-id="df187-125">String</span></span>|<span data-ttu-id="df187-126">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="df187-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="df187-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="df187-127">\*.crt</span></span> | <span data-ttu-id="df187-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="df187-128">\*.p7b</span></span> | <span data-ttu-id="df187-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="df187-129">\*.bin).</span></span>|
|<span data-ttu-id="df187-130">value</span><span class="sxs-lookup"><span data-stu-id="df187-130">value</span></span>|<span data-ttu-id="df187-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df187-131">String</span></span>|<span data-ttu-id="df187-132">Valor.</span><span class="sxs-lookup"><span data-stu-id="df187-132">Value.</span></span> <span data-ttu-id="df187-133">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="df187-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="df187-134">Relações</span><span class="sxs-lookup"><span data-stu-id="df187-134">Relationships</span></span>
<span data-ttu-id="df187-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df187-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df187-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df187-136">JSON Representation</span></span>
<span data-ttu-id="df187-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df187-137">Here is a JSON representation of the resource.</span></span>
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




