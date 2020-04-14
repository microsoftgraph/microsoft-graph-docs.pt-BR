---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8ed09ee79b8a5607f4aec0647ed7d221ee407e5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459272"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="e5177-103">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="e5177-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="e5177-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5177-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5177-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5177-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5177-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5177-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5177-107">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="e5177-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="e5177-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5177-108">Properties</span></span>
|<span data-ttu-id="e5177-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5177-109">Property</span></span>|<span data-ttu-id="e5177-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5177-110">Type</span></span>|<span data-ttu-id="e5177-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5177-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5177-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="e5177-112">schemaItemKey</span></span>|<span data-ttu-id="e5177-113">String</span><span class="sxs-lookup"><span data-stu-id="e5177-113">String</span></span>|<span data-ttu-id="e5177-114">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="e5177-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="e5177-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e5177-115">displayName</span></span>|<span data-ttu-id="e5177-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5177-116">String</span></span>|<span data-ttu-id="e5177-117">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="e5177-117">Human readable name</span></span>|
|<span data-ttu-id="e5177-118">description</span><span class="sxs-lookup"><span data-stu-id="e5177-118">description</span></span>|<span data-ttu-id="e5177-119">String</span><span class="sxs-lookup"><span data-stu-id="e5177-119">String</span></span>|<span data-ttu-id="e5177-120">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5177-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="e5177-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="e5177-121">defaultBoolValue</span></span>|<span data-ttu-id="e5177-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="e5177-122">Boolean</span></span>|<span data-ttu-id="e5177-123">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5177-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5177-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="e5177-124">defaultIntValue</span></span>|<span data-ttu-id="e5177-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e5177-125">Int32</span></span>|<span data-ttu-id="e5177-126">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5177-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5177-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="e5177-127">defaultStringValue</span></span>|<span data-ttu-id="e5177-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5177-128">String</span></span>|<span data-ttu-id="e5177-129">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5177-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5177-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="e5177-130">defaultStringArrayValue</span></span>|<span data-ttu-id="e5177-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e5177-131">String collection</span></span>|<span data-ttu-id="e5177-132">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5177-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e5177-133">dataType</span><span class="sxs-lookup"><span data-stu-id="e5177-133">dataType</span></span>|[<span data-ttu-id="e5177-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="e5177-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="e5177-135">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="e5177-135">The type of value this item describes.</span></span> <span data-ttu-id="e5177-136">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="e5177-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="e5177-137">selections</span><span class="sxs-lookup"><span data-stu-id="e5177-137">selections</span></span>|<span data-ttu-id="e5177-138">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e5177-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e5177-139">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="e5177-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5177-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e5177-140">Relationships</span></span>
<span data-ttu-id="e5177-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5177-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5177-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5177-142">JSON Representation</span></span>
<span data-ttu-id="e5177-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5177-143">Here is a JSON representation of the resource.</span></span>
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



