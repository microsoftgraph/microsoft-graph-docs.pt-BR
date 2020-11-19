---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67ab2980b8fb228803eee955302f9db69065dd15
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273085"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="9ab1f-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="9ab1f-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="9ab1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ab1f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ab1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab1f-107">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="9ab1f-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ab1f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ab1f-109">Properties</span></span>
|<span data-ttu-id="9ab1f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ab1f-110">Property</span></span>|<span data-ttu-id="9ab1f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ab1f-111">Type</span></span>|<span data-ttu-id="9ab1f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab1f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab1f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9ab1f-113">displayName</span></span>|<span data-ttu-id="9ab1f-114">String</span><span class="sxs-lookup"><span data-stu-id="9ab1f-114">String</span></span>|<span data-ttu-id="9ab1f-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-115">Display Name.</span></span> <span data-ttu-id="9ab1f-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ab1f-117">description</span><span class="sxs-lookup"><span data-stu-id="9ab1f-117">description</span></span>|<span data-ttu-id="9ab1f-118">String</span><span class="sxs-lookup"><span data-stu-id="9ab1f-118">String</span></span>|<span data-ttu-id="9ab1f-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-119">Description.</span></span> <span data-ttu-id="9ab1f-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ab1f-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9ab1f-121">omaUri</span></span>|<span data-ttu-id="9ab1f-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab1f-122">String</span></span>|<span data-ttu-id="9ab1f-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-123">OMA.</span></span> <span data-ttu-id="9ab1f-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ab1f-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9ab1f-125">isEncrypted</span></span>|<span data-ttu-id="9ab1f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ab1f-126">Boolean</span></span>|<span data-ttu-id="9ab1f-127">Indica se o campo de valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="9ab1f-128">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ab1f-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ab1f-129">valor</span><span class="sxs-lookup"><span data-stu-id="9ab1f-129">value</span></span>|<span data-ttu-id="9ab1f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9ab1f-130">Int32</span></span>|<span data-ttu-id="9ab1f-131">Valor.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-131">Value.</span></span>|
|<span data-ttu-id="9ab1f-132">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="9ab1f-132">isReadOnly</span></span>|<span data-ttu-id="9ab1f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ab1f-133">Boolean</span></span>|<span data-ttu-id="9ab1f-134">Definindo como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de Set</span><span class="sxs-lookup"><span data-stu-id="9ab1f-134">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ab1f-135">Relações</span><span class="sxs-lookup"><span data-stu-id="9ab1f-135">Relationships</span></span>
<span data-ttu-id="9ab1f-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ab1f-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ab1f-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ab1f-137">JSON Representation</span></span>
<span data-ttu-id="9ab1f-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ab1f-138">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "value": 1024,
  "isReadOnly": true
}
```




