---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 829f73ec2d5eb205e6cacdb46ee209760334cb3a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788440"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="e1e59-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="e1e59-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="e1e59-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1e59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1e59-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1e59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1e59-106">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e1e59-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="e1e59-107">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1e59-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1e59-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1e59-108">Properties</span></span>
|<span data-ttu-id="e1e59-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1e59-109">Property</span></span>|<span data-ttu-id="e1e59-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1e59-110">Type</span></span>|<span data-ttu-id="e1e59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1e59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1e59-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e1e59-112">displayName</span></span>|<span data-ttu-id="e1e59-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1e59-113">String</span></span>|<span data-ttu-id="e1e59-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e1e59-114">Display Name.</span></span> <span data-ttu-id="e1e59-115">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1e59-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1e59-116">description</span><span class="sxs-lookup"><span data-stu-id="e1e59-116">description</span></span>|<span data-ttu-id="e1e59-117">String</span><span class="sxs-lookup"><span data-stu-id="e1e59-117">String</span></span>|<span data-ttu-id="e1e59-118">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e1e59-118">Description.</span></span> <span data-ttu-id="e1e59-119">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1e59-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1e59-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="e1e59-120">omaUri</span></span>|<span data-ttu-id="e1e59-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1e59-121">String</span></span>|<span data-ttu-id="e1e59-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="e1e59-122">OMA.</span></span> <span data-ttu-id="e1e59-123">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1e59-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1e59-124">valor</span><span class="sxs-lookup"><span data-stu-id="e1e59-124">value</span></span>|<span data-ttu-id="e1e59-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e1e59-125">Int32</span></span>|<span data-ttu-id="e1e59-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="e1e59-126">Value.</span></span>|
|<span data-ttu-id="e1e59-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="e1e59-127">isReadOnly</span></span>|<span data-ttu-id="e1e59-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1e59-128">Boolean</span></span>|<span data-ttu-id="e1e59-129">Definindo como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de Set</span><span class="sxs-lookup"><span data-stu-id="e1e59-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1e59-130">Relações</span><span class="sxs-lookup"><span data-stu-id="e1e59-130">Relationships</span></span>
<span data-ttu-id="e1e59-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1e59-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1e59-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1e59-132">JSON Representation</span></span>
<span data-ttu-id="e1e59-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1e59-133">Here is a JSON representation of the resource.</span></span>
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



