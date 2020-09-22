---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64fbfca7b5fc101ea7ea64d4545257354d4157e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010168"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="5a334-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="5a334-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="5a334-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a334-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a334-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a334-107">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="5a334-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="5a334-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5a334-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a334-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a334-109">Properties</span></span>
|<span data-ttu-id="5a334-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a334-110">Property</span></span>|<span data-ttu-id="5a334-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a334-111">Type</span></span>|<span data-ttu-id="5a334-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a334-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a334-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5a334-113">displayName</span></span>|<span data-ttu-id="5a334-114">String</span><span class="sxs-lookup"><span data-stu-id="5a334-114">String</span></span>|<span data-ttu-id="5a334-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="5a334-115">Display Name.</span></span> <span data-ttu-id="5a334-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5a334-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5a334-117">description</span><span class="sxs-lookup"><span data-stu-id="5a334-117">description</span></span>|<span data-ttu-id="5a334-118">String</span><span class="sxs-lookup"><span data-stu-id="5a334-118">String</span></span>|<span data-ttu-id="5a334-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="5a334-119">Description.</span></span> <span data-ttu-id="5a334-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5a334-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5a334-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="5a334-121">omaUri</span></span>|<span data-ttu-id="5a334-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a334-122">String</span></span>|<span data-ttu-id="5a334-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="5a334-123">OMA.</span></span> <span data-ttu-id="5a334-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5a334-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5a334-125">valor</span><span class="sxs-lookup"><span data-stu-id="5a334-125">value</span></span>|<span data-ttu-id="5a334-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5a334-126">Int32</span></span>|<span data-ttu-id="5a334-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="5a334-127">Value.</span></span>|
|<span data-ttu-id="5a334-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="5a334-128">isReadOnly</span></span>|<span data-ttu-id="5a334-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a334-129">Boolean</span></span>|<span data-ttu-id="5a334-130">Definindo como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de Set</span><span class="sxs-lookup"><span data-stu-id="5a334-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a334-131">Relações</span><span class="sxs-lookup"><span data-stu-id="5a334-131">Relationships</span></span>
<span data-ttu-id="5a334-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a334-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a334-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a334-133">JSON Representation</span></span>
<span data-ttu-id="5a334-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a334-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024,
  "isReadOnly": true
}
```






