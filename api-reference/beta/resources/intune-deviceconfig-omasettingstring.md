---
title: Tipo de recurso omaSettingString
description: Definição de cadeia de caracteres para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b20f71bb7d5e188303c742efce96b23f89f698c0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867375"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="9900e-103">Tipo de recurso omaSettingString</span><span class="sxs-lookup"><span data-stu-id="9900e-103">omaSettingString resource type</span></span>

<span data-ttu-id="9900e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9900e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9900e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9900e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9900e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9900e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9900e-107">Definição de cadeia de caracteres para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="9900e-107">OMA Settings String definition.</span></span>


<span data-ttu-id="9900e-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9900e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9900e-109">Properties</span></span>
|<span data-ttu-id="9900e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9900e-110">Property</span></span>|<span data-ttu-id="9900e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9900e-111">Type</span></span>|<span data-ttu-id="9900e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9900e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9900e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9900e-113">displayName</span></span>|<span data-ttu-id="9900e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9900e-114">String</span></span>|<span data-ttu-id="9900e-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9900e-115">Display Name.</span></span> <span data-ttu-id="9900e-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9900e-117">description</span><span class="sxs-lookup"><span data-stu-id="9900e-117">description</span></span>|<span data-ttu-id="9900e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9900e-118">String</span></span>|<span data-ttu-id="9900e-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="9900e-119">Description.</span></span> <span data-ttu-id="9900e-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9900e-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9900e-121">omaUri</span></span>|<span data-ttu-id="9900e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9900e-122">String</span></span>|<span data-ttu-id="9900e-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="9900e-123">OMA.</span></span> <span data-ttu-id="9900e-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9900e-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="9900e-125">secretReferenceValueId</span></span>|<span data-ttu-id="9900e-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9900e-126">String</span></span>|<span data-ttu-id="9900e-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="9900e-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="9900e-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9900e-128">This property is read-only.</span></span> <span data-ttu-id="9900e-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9900e-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9900e-130">isEncrypted</span></span>|<span data-ttu-id="9900e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9900e-131">Boolean</span></span>|<span data-ttu-id="9900e-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="9900e-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="9900e-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9900e-133">This property is read-only.</span></span> <span data-ttu-id="9900e-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9900e-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9900e-135">value</span><span class="sxs-lookup"><span data-stu-id="9900e-135">value</span></span>|<span data-ttu-id="9900e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9900e-136">String</span></span>|<span data-ttu-id="9900e-137">Valor.</span><span class="sxs-lookup"><span data-stu-id="9900e-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9900e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="9900e-138">Relationships</span></span>
<span data-ttu-id="9900e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9900e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9900e-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9900e-140">JSON Representation</span></span>
<span data-ttu-id="9900e-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9900e-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String"
}
```




