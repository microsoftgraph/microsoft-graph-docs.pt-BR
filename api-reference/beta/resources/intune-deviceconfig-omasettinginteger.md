---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e5dccc9a0b4329d0f871fa997c627b73ee4bdfc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722954"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="cb242-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="cb242-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="cb242-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb242-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb242-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb242-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb242-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb242-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb242-107">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="cb242-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="cb242-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb242-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb242-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb242-109">Properties</span></span>
|<span data-ttu-id="cb242-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb242-110">Property</span></span>|<span data-ttu-id="cb242-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb242-111">Type</span></span>|<span data-ttu-id="cb242-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb242-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb242-113">displayName</span><span class="sxs-lookup"><span data-stu-id="cb242-113">displayName</span></span>|<span data-ttu-id="cb242-114">String</span><span class="sxs-lookup"><span data-stu-id="cb242-114">String</span></span>|<span data-ttu-id="cb242-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="cb242-115">Display Name.</span></span> <span data-ttu-id="cb242-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb242-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb242-117">description</span><span class="sxs-lookup"><span data-stu-id="cb242-117">description</span></span>|<span data-ttu-id="cb242-118">String</span><span class="sxs-lookup"><span data-stu-id="cb242-118">String</span></span>|<span data-ttu-id="cb242-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="cb242-119">Description.</span></span> <span data-ttu-id="cb242-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb242-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb242-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="cb242-121">omaUri</span></span>|<span data-ttu-id="cb242-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb242-122">String</span></span>|<span data-ttu-id="cb242-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="cb242-123">OMA.</span></span> <span data-ttu-id="cb242-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb242-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb242-125">valor</span><span class="sxs-lookup"><span data-stu-id="cb242-125">value</span></span>|<span data-ttu-id="cb242-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cb242-126">Int32</span></span>|<span data-ttu-id="cb242-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="cb242-127">Value.</span></span>|
|<span data-ttu-id="cb242-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="cb242-128">isReadOnly</span></span>|<span data-ttu-id="cb242-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb242-129">Boolean</span></span>|<span data-ttu-id="cb242-130">Definindo como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de Set</span><span class="sxs-lookup"><span data-stu-id="cb242-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb242-131">Relações</span><span class="sxs-lookup"><span data-stu-id="cb242-131">Relationships</span></span>
<span data-ttu-id="cb242-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb242-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb242-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb242-133">JSON Representation</span></span>
<span data-ttu-id="cb242-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb242-134">Here is a JSON representation of the resource.</span></span>
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





