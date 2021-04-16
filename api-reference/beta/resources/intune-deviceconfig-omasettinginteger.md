---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19db5504d276c748d720803ba201c555752e2f33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867389"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="23711-103">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="23711-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="23711-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23711-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23711-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23711-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23711-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23711-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23711-107">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="23711-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="23711-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23711-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23711-109">Properties</span></span>
|<span data-ttu-id="23711-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23711-110">Property</span></span>|<span data-ttu-id="23711-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="23711-111">Type</span></span>|<span data-ttu-id="23711-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23711-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23711-113">displayName</span><span class="sxs-lookup"><span data-stu-id="23711-113">displayName</span></span>|<span data-ttu-id="23711-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23711-114">String</span></span>|<span data-ttu-id="23711-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="23711-115">Display Name.</span></span> <span data-ttu-id="23711-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="23711-117">description</span><span class="sxs-lookup"><span data-stu-id="23711-117">description</span></span>|<span data-ttu-id="23711-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23711-118">String</span></span>|<span data-ttu-id="23711-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="23711-119">Description.</span></span> <span data-ttu-id="23711-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="23711-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="23711-121">omaUri</span></span>|<span data-ttu-id="23711-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23711-122">String</span></span>|<span data-ttu-id="23711-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="23711-123">OMA.</span></span> <span data-ttu-id="23711-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="23711-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="23711-125">secretReferenceValueId</span></span>|<span data-ttu-id="23711-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="23711-126">String</span></span>|<span data-ttu-id="23711-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="23711-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="23711-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23711-128">This property is read-only.</span></span> <span data-ttu-id="23711-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="23711-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="23711-130">isEncrypted</span></span>|<span data-ttu-id="23711-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="23711-131">Boolean</span></span>|<span data-ttu-id="23711-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="23711-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="23711-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23711-133">This property is read-only.</span></span> <span data-ttu-id="23711-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="23711-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="23711-135">valor</span><span class="sxs-lookup"><span data-stu-id="23711-135">value</span></span>|<span data-ttu-id="23711-136">Int32</span><span class="sxs-lookup"><span data-stu-id="23711-136">Int32</span></span>|<span data-ttu-id="23711-137">Valor.</span><span class="sxs-lookup"><span data-stu-id="23711-137">Value.</span></span>|
|<span data-ttu-id="23711-138">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="23711-138">isReadOnly</span></span>|<span data-ttu-id="23711-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="23711-139">Boolean</span></span>|<span data-ttu-id="23711-140">Ao definir como true, o CSP (provedor de serviços de configuração) especificado no OMA-URI executará um get, em vez de definir</span><span class="sxs-lookup"><span data-stu-id="23711-140">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="23711-141">Relações</span><span class="sxs-lookup"><span data-stu-id="23711-141">Relationships</span></span>
<span data-ttu-id="23711-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23711-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23711-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23711-143">JSON Representation</span></span>
<span data-ttu-id="23711-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23711-144">Here is a JSON representation of the resource.</span></span>
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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 1024,
  "isReadOnly": true
}
```




