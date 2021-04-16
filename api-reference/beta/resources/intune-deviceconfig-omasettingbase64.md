---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8729dd6251f9dbaf062fbfee3d024de265565020
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867452"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="ca3dd-103">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="ca3dd-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="ca3dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca3dd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3dd-107">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="ca3dd-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca3dd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca3dd-109">Properties</span></span>
|<span data-ttu-id="ca3dd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca3dd-110">Property</span></span>|<span data-ttu-id="ca3dd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca3dd-111">Type</span></span>|<span data-ttu-id="ca3dd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca3dd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3dd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ca3dd-113">displayName</span></span>|<span data-ttu-id="ca3dd-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-114">String</span></span>|<span data-ttu-id="ca3dd-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-115">Display Name.</span></span> <span data-ttu-id="ca3dd-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ca3dd-117">description</span><span class="sxs-lookup"><span data-stu-id="ca3dd-117">description</span></span>|<span data-ttu-id="ca3dd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-118">String</span></span>|<span data-ttu-id="ca3dd-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-119">Description.</span></span> <span data-ttu-id="ca3dd-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ca3dd-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ca3dd-121">omaUri</span></span>|<span data-ttu-id="ca3dd-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-122">String</span></span>|<span data-ttu-id="ca3dd-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-123">OMA.</span></span> <span data-ttu-id="ca3dd-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ca3dd-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="ca3dd-125">secretReferenceValueId</span></span>|<span data-ttu-id="ca3dd-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-126">String</span></span>|<span data-ttu-id="ca3dd-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="ca3dd-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-128">This property is read-only.</span></span> <span data-ttu-id="ca3dd-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ca3dd-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ca3dd-130">isEncrypted</span></span>|<span data-ttu-id="ca3dd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3dd-131">Boolean</span></span>|<span data-ttu-id="ca3dd-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="ca3dd-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-133">This property is read-only.</span></span> <span data-ttu-id="ca3dd-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ca3dd-135">fileName</span><span class="sxs-lookup"><span data-stu-id="ca3dd-135">fileName</span></span>|<span data-ttu-id="ca3dd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-136">String</span></span>|<span data-ttu-id="ca3dd-137">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="ca3dd-137">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="ca3dd-138">\*.crt</span><span class="sxs-lookup"><span data-stu-id="ca3dd-138">\*.crt</span></span> | <span data-ttu-id="ca3dd-139">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="ca3dd-139">\*.p7b</span></span> | <span data-ttu-id="ca3dd-140">\*.bin).</span><span class="sxs-lookup"><span data-stu-id="ca3dd-140">\*.bin).</span></span>|
|<span data-ttu-id="ca3dd-141">value</span><span class="sxs-lookup"><span data-stu-id="ca3dd-141">value</span></span>|<span data-ttu-id="ca3dd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca3dd-142">String</span></span>|<span data-ttu-id="ca3dd-143">Valor.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-143">Value.</span></span> <span data-ttu-id="ca3dd-144">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="ca3dd-144">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca3dd-145">Relações</span><span class="sxs-lookup"><span data-stu-id="ca3dd-145">Relationships</span></span>
<span data-ttu-id="ca3dd-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca3dd-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca3dd-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca3dd-147">JSON Representation</span></span>
<span data-ttu-id="ca3dd-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca3dd-148">Here is a JSON representation of the resource.</span></span>
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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




