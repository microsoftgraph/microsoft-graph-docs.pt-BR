---
title: Tipo de recurso omaSettingBoolean
description: Definição booliana para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e1118001a06ff19439d5d0b1a3970b358235f4d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867438"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="81f20-103">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="81f20-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="81f20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81f20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81f20-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81f20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81f20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81f20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81f20-107">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="81f20-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="81f20-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81f20-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81f20-109">Properties</span></span>
|<span data-ttu-id="81f20-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f20-110">Property</span></span>|<span data-ttu-id="81f20-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f20-111">Type</span></span>|<span data-ttu-id="81f20-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f20-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f20-113">displayName</span><span class="sxs-lookup"><span data-stu-id="81f20-113">displayName</span></span>|<span data-ttu-id="81f20-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f20-114">String</span></span>|<span data-ttu-id="81f20-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="81f20-115">Display Name.</span></span> <span data-ttu-id="81f20-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f20-117">description</span><span class="sxs-lookup"><span data-stu-id="81f20-117">description</span></span>|<span data-ttu-id="81f20-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f20-118">String</span></span>|<span data-ttu-id="81f20-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="81f20-119">Description.</span></span> <span data-ttu-id="81f20-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f20-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="81f20-121">omaUri</span></span>|<span data-ttu-id="81f20-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f20-122">String</span></span>|<span data-ttu-id="81f20-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="81f20-123">OMA.</span></span> <span data-ttu-id="81f20-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f20-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="81f20-125">secretReferenceValueId</span></span>|<span data-ttu-id="81f20-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="81f20-126">String</span></span>|<span data-ttu-id="81f20-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="81f20-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="81f20-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81f20-128">This property is read-only.</span></span> <span data-ttu-id="81f20-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f20-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="81f20-130">isEncrypted</span></span>|<span data-ttu-id="81f20-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="81f20-131">Boolean</span></span>|<span data-ttu-id="81f20-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="81f20-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="81f20-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81f20-133">This property is read-only.</span></span> <span data-ttu-id="81f20-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81f20-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81f20-135">value</span><span class="sxs-lookup"><span data-stu-id="81f20-135">value</span></span>|<span data-ttu-id="81f20-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="81f20-136">Boolean</span></span>|<span data-ttu-id="81f20-137">Valor.</span><span class="sxs-lookup"><span data-stu-id="81f20-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81f20-138">Relações</span><span class="sxs-lookup"><span data-stu-id="81f20-138">Relationships</span></span>
<span data-ttu-id="81f20-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81f20-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81f20-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81f20-140">JSON Representation</span></span>
<span data-ttu-id="81f20-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81f20-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": true
}
```




