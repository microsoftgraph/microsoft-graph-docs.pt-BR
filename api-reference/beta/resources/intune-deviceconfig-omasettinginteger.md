---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b0dc774d5ab95733337719014f9db93bc393d71
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462985"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="1539a-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="1539a-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="1539a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1539a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1539a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1539a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1539a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1539a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1539a-107">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1539a-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="1539a-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1539a-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1539a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1539a-109">Properties</span></span>
|<span data-ttu-id="1539a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1539a-110">Property</span></span>|<span data-ttu-id="1539a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1539a-111">Type</span></span>|<span data-ttu-id="1539a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1539a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1539a-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1539a-113">displayName</span></span>|<span data-ttu-id="1539a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1539a-114">String</span></span>|<span data-ttu-id="1539a-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1539a-115">Display Name.</span></span> <span data-ttu-id="1539a-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1539a-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1539a-117">description</span><span class="sxs-lookup"><span data-stu-id="1539a-117">description</span></span>|<span data-ttu-id="1539a-118">String</span><span class="sxs-lookup"><span data-stu-id="1539a-118">String</span></span>|<span data-ttu-id="1539a-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1539a-119">Description.</span></span> <span data-ttu-id="1539a-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1539a-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1539a-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="1539a-121">omaUri</span></span>|<span data-ttu-id="1539a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1539a-122">String</span></span>|<span data-ttu-id="1539a-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="1539a-123">OMA.</span></span> <span data-ttu-id="1539a-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1539a-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1539a-125">valor</span><span class="sxs-lookup"><span data-stu-id="1539a-125">value</span></span>|<span data-ttu-id="1539a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1539a-126">Int32</span></span>|<span data-ttu-id="1539a-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="1539a-127">Value.</span></span>|
|<span data-ttu-id="1539a-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="1539a-128">isReadOnly</span></span>|<span data-ttu-id="1539a-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="1539a-129">Boolean</span></span>|<span data-ttu-id="1539a-130">Definindo como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de Set</span><span class="sxs-lookup"><span data-stu-id="1539a-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="1539a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="1539a-131">Relationships</span></span>
<span data-ttu-id="1539a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1539a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1539a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1539a-133">JSON Representation</span></span>
<span data-ttu-id="1539a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1539a-134">Here is a JSON representation of the resource.</span></span>
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



