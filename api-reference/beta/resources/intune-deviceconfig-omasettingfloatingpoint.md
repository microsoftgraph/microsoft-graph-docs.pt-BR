---
title: Tipo de recurso omaSettingFloatingPoint
description: Definição de ponto flutuante para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 43c3c73d01eb5e2e44c5f5a0a9e85c2e6577262e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273120"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="9b37f-103">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="9b37f-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="9b37f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b37f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b37f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b37f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b37f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b37f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b37f-107">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="9b37f-107">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="9b37f-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9b37f-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b37f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b37f-109">Properties</span></span>
|<span data-ttu-id="9b37f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b37f-110">Property</span></span>|<span data-ttu-id="9b37f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b37f-111">Type</span></span>|<span data-ttu-id="9b37f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b37f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b37f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9b37f-113">displayName</span></span>|<span data-ttu-id="9b37f-114">String</span><span class="sxs-lookup"><span data-stu-id="9b37f-114">String</span></span>|<span data-ttu-id="9b37f-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9b37f-115">Display Name.</span></span> <span data-ttu-id="9b37f-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9b37f-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9b37f-117">description</span><span class="sxs-lookup"><span data-stu-id="9b37f-117">description</span></span>|<span data-ttu-id="9b37f-118">String</span><span class="sxs-lookup"><span data-stu-id="9b37f-118">String</span></span>|<span data-ttu-id="9b37f-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="9b37f-119">Description.</span></span> <span data-ttu-id="9b37f-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9b37f-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9b37f-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9b37f-121">omaUri</span></span>|<span data-ttu-id="9b37f-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b37f-122">String</span></span>|<span data-ttu-id="9b37f-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="9b37f-123">OMA.</span></span> <span data-ttu-id="9b37f-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9b37f-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9b37f-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9b37f-125">isEncrypted</span></span>|<span data-ttu-id="9b37f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b37f-126">Boolean</span></span>|<span data-ttu-id="9b37f-127">Indica se o campo de valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="9b37f-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="9b37f-128">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9b37f-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9b37f-129">value</span><span class="sxs-lookup"><span data-stu-id="9b37f-129">value</span></span>|<span data-ttu-id="9b37f-130">Single</span><span class="sxs-lookup"><span data-stu-id="9b37f-130">Single</span></span>|<span data-ttu-id="9b37f-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="9b37f-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b37f-132">Relações</span><span class="sxs-lookup"><span data-stu-id="9b37f-132">Relationships</span></span>
<span data-ttu-id="9b37f-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b37f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b37f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b37f-134">JSON Representation</span></span>
<span data-ttu-id="9b37f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b37f-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "isEncrypted": true,
  "value": 4.2
}
```




