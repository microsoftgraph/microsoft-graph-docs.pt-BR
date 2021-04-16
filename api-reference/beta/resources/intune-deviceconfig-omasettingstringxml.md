---
title: Tipo de recurso omaSettingStringXml
description: Definição de StringXML para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b899a076a291061649adab4724a9108d982886f5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867368"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="719d3-103">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="719d3-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="719d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="719d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="719d3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="719d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="719d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="719d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="719d3-107">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="719d3-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="719d3-108">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="719d3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="719d3-109">Properties</span></span>
|<span data-ttu-id="719d3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="719d3-110">Property</span></span>|<span data-ttu-id="719d3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="719d3-111">Type</span></span>|<span data-ttu-id="719d3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="719d3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="719d3-113">displayName</span><span class="sxs-lookup"><span data-stu-id="719d3-113">displayName</span></span>|<span data-ttu-id="719d3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="719d3-114">String</span></span>|<span data-ttu-id="719d3-115">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="719d3-115">Display Name.</span></span> <span data-ttu-id="719d3-116">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="719d3-117">description</span><span class="sxs-lookup"><span data-stu-id="719d3-117">description</span></span>|<span data-ttu-id="719d3-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="719d3-118">String</span></span>|<span data-ttu-id="719d3-119">Descrição.</span><span class="sxs-lookup"><span data-stu-id="719d3-119">Description.</span></span> <span data-ttu-id="719d3-120">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="719d3-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="719d3-121">omaUri</span></span>|<span data-ttu-id="719d3-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="719d3-122">String</span></span>|<span data-ttu-id="719d3-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="719d3-123">OMA.</span></span> <span data-ttu-id="719d3-124">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="719d3-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="719d3-125">secretReferenceValueId</span></span>|<span data-ttu-id="719d3-126">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="719d3-126">String</span></span>|<span data-ttu-id="719d3-127">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="719d3-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="719d3-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="719d3-128">This property is read-only.</span></span> <span data-ttu-id="719d3-129">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="719d3-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="719d3-130">isEncrypted</span></span>|<span data-ttu-id="719d3-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="719d3-131">Boolean</span></span>|<span data-ttu-id="719d3-132">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="719d3-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="719d3-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="719d3-133">This property is read-only.</span></span> <span data-ttu-id="719d3-134">Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="719d3-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="719d3-135">fileName</span><span class="sxs-lookup"><span data-stu-id="719d3-135">fileName</span></span>|<span data-ttu-id="719d3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="719d3-136">String</span></span>|<span data-ttu-id="719d3-137">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="719d3-137">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="719d3-138">valor</span><span class="sxs-lookup"><span data-stu-id="719d3-138">value</span></span>|<span data-ttu-id="719d3-139">Binário</span><span class="sxs-lookup"><span data-stu-id="719d3-139">Binary</span></span>|<span data-ttu-id="719d3-140">Valor.</span><span class="sxs-lookup"><span data-stu-id="719d3-140">Value.</span></span> <span data-ttu-id="719d3-141">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="719d3-141">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="719d3-142">Relações</span><span class="sxs-lookup"><span data-stu-id="719d3-142">Relationships</span></span>
<span data-ttu-id="719d3-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="719d3-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="719d3-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="719d3-144">JSON Representation</span></span>
<span data-ttu-id="719d3-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="719d3-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "binary"
}
```




