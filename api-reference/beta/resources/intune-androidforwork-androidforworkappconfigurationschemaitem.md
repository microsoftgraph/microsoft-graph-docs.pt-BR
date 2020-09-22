---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13af3b581498a4285773b2fda02d5596127c3012
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019667"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="e5714-103">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="e5714-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="e5714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5714-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5714-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5714-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5714-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5714-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5714-107">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="e5714-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="e5714-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5714-108">Properties</span></span>
|<span data-ttu-id="e5714-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5714-109">Property</span></span>|<span data-ttu-id="e5714-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5714-110">Type</span></span>|<span data-ttu-id="e5714-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5714-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5714-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="e5714-112">schemaItemKey</span></span>|<span data-ttu-id="e5714-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5714-113">String</span></span>|<span data-ttu-id="e5714-114">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="e5714-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="e5714-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e5714-115">displayName</span></span>|<span data-ttu-id="e5714-116">String</span><span class="sxs-lookup"><span data-stu-id="e5714-116">String</span></span>|<span data-ttu-id="e5714-117">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="e5714-117">Human readable name</span></span>|
|<span data-ttu-id="e5714-118">description</span><span class="sxs-lookup"><span data-stu-id="e5714-118">description</span></span>|<span data-ttu-id="e5714-119">String</span><span class="sxs-lookup"><span data-stu-id="e5714-119">String</span></span>|<span data-ttu-id="e5714-120">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5714-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="e5714-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="e5714-121">defaultBoolValue</span></span>|<span data-ttu-id="e5714-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="e5714-122">Boolean</span></span>|<span data-ttu-id="e5714-123">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5714-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5714-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="e5714-124">defaultIntValue</span></span>|<span data-ttu-id="e5714-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e5714-125">Int32</span></span>|<span data-ttu-id="e5714-126">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5714-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5714-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="e5714-127">defaultStringValue</span></span>|<span data-ttu-id="e5714-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5714-128">String</span></span>|<span data-ttu-id="e5714-129">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5714-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5714-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="e5714-130">defaultStringArrayValue</span></span>|<span data-ttu-id="e5714-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e5714-131">String collection</span></span>|<span data-ttu-id="e5714-132">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5714-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5714-133">dataType</span><span class="sxs-lookup"><span data-stu-id="e5714-133">dataType</span></span>|[<span data-ttu-id="e5714-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="e5714-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="e5714-135">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="e5714-135">The type of value this item describes.</span></span> <span data-ttu-id="e5714-136">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="e5714-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="e5714-137">selections</span><span class="sxs-lookup"><span data-stu-id="e5714-137">selections</span></span>|<span data-ttu-id="e5714-138">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e5714-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e5714-139">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="e5714-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5714-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e5714-140">Relationships</span></span>
<span data-ttu-id="e5714-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5714-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5714-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5714-142">JSON Representation</span></span>
<span data-ttu-id="e5714-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5714-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```






