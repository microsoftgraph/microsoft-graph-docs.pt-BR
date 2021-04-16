---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30ed623b5fc59b9a96c0e37e8b2b1fcfc77e7b13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867424"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="89da6-103">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="89da6-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="89da6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89da6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89da6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89da6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89da6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89da6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89da6-107">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="89da6-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="89da6-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89da6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89da6-109">Properties</span></span>
|<span data-ttu-id="89da6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89da6-110">Property</span></span>|<span data-ttu-id="89da6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="89da6-111">Type</span></span>|<span data-ttu-id="89da6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="89da6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89da6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="89da6-113">displayName</span></span>|<span data-ttu-id="89da6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89da6-114">String</span></span>|<span data-ttu-id="89da6-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="89da6-115">Display Name.</span></span> <span data-ttu-id="89da6-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89da6-117">description</span><span class="sxs-lookup"><span data-stu-id="89da6-117">description</span></span>|<span data-ttu-id="89da6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89da6-118">String</span></span>|<span data-ttu-id="89da6-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="89da6-119">Description.</span></span> <span data-ttu-id="89da6-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89da6-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="89da6-121">omaUri</span></span>|<span data-ttu-id="89da6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89da6-122">String</span></span>|<span data-ttu-id="89da6-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="89da6-123">OMA.</span></span> <span data-ttu-id="89da6-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89da6-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="89da6-125">secretReferenceValueId</span></span>|<span data-ttu-id="89da6-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="89da6-126">String</span></span>|<span data-ttu-id="89da6-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="89da6-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="89da6-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89da6-128">This property is read-only.</span></span> <span data-ttu-id="89da6-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89da6-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="89da6-130">isEncrypted</span></span>|<span data-ttu-id="89da6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="89da6-131">Boolean</span></span>|<span data-ttu-id="89da6-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="89da6-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="89da6-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89da6-133">This property is read-only.</span></span> <span data-ttu-id="89da6-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="89da6-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="89da6-135">value</span><span class="sxs-lookup"><span data-stu-id="89da6-135">value</span></span>|<span data-ttu-id="89da6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89da6-136">DateTimeOffset</span></span>|<span data-ttu-id="89da6-137">Valor.</span><span class="sxs-lookup"><span data-stu-id="89da6-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89da6-138">Relações</span><span class="sxs-lookup"><span data-stu-id="89da6-138">Relationships</span></span>
<span data-ttu-id="89da6-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89da6-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89da6-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89da6-140">JSON Representation</span></span>
<span data-ttu-id="89da6-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89da6-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String (timestamp)"
}
```




