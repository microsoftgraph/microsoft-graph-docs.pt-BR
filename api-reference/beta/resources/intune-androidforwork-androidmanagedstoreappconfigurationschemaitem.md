---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6db7a9958599cbc073fa17eef542559a65af2b8e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799329"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="4b1e5-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="4b1e5-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="4b1e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b1e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b1e5-106">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="4b1e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b1e5-107">Properties</span></span>
|<span data-ttu-id="4b1e5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b1e5-108">Property</span></span>|<span data-ttu-id="4b1e5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-109">Type</span></span>|<span data-ttu-id="4b1e5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b1e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b1e5-111">índice</span><span class="sxs-lookup"><span data-stu-id="4b1e5-111">index</span></span>|<span data-ttu-id="4b1e5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4b1e5-112">Int32</span></span>|<span data-ttu-id="4b1e5-113">Índice exclusivo que o aplicativo usa para manter itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="4b1e5-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="4b1e5-114">parentIndex</span><span class="sxs-lookup"><span data-stu-id="4b1e5-114">parentIndex</span></span>|<span data-ttu-id="4b1e5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="4b1e5-115">Int32</span></span>|<span data-ttu-id="4b1e5-116">Índice do item de esquema pai para rastrear itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="4b1e5-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="4b1e5-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="4b1e5-117">schemaItemKey</span></span>|<span data-ttu-id="4b1e5-118">String</span><span class="sxs-lookup"><span data-stu-id="4b1e5-118">String</span></span>|<span data-ttu-id="4b1e5-119">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="4b1e5-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="4b1e5-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4b1e5-120">displayName</span></span>|<span data-ttu-id="4b1e5-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b1e5-121">String</span></span>|<span data-ttu-id="4b1e5-122">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="4b1e5-122">Human readable name</span></span>|
|<span data-ttu-id="4b1e5-123">description</span><span class="sxs-lookup"><span data-stu-id="4b1e5-123">description</span></span>|<span data-ttu-id="4b1e5-124">String</span><span class="sxs-lookup"><span data-stu-id="4b1e5-124">String</span></span>|<span data-ttu-id="4b1e5-125">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="4b1e5-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="4b1e5-126">defaultBoolValue</span></span>|<span data-ttu-id="4b1e5-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b1e5-127">Boolean</span></span>|<span data-ttu-id="4b1e5-128">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4b1e5-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="4b1e5-129">defaultIntValue</span></span>|<span data-ttu-id="4b1e5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="4b1e5-130">Int32</span></span>|<span data-ttu-id="4b1e5-131">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4b1e5-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="4b1e5-132">defaultStringValue</span></span>|<span data-ttu-id="4b1e5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b1e5-133">String</span></span>|<span data-ttu-id="4b1e5-134">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4b1e5-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="4b1e5-135">defaultStringArrayValue</span></span>|<span data-ttu-id="4b1e5-136">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4b1e5-136">String collection</span></span>|<span data-ttu-id="4b1e5-137">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b1e5-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4b1e5-138">dataType</span><span class="sxs-lookup"><span data-stu-id="4b1e5-138">dataType</span></span>|[<span data-ttu-id="4b1e5-139">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="4b1e5-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="4b1e5-140">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-140">The type of value this item describes.</span></span> <span data-ttu-id="4b1e5-141">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="4b1e5-142">selections</span><span class="sxs-lookup"><span data-stu-id="4b1e5-142">selections</span></span>|<span data-ttu-id="4b1e5-143">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4b1e5-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4b1e5-144">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="4b1e5-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1e5-145">Relações</span><span class="sxs-lookup"><span data-stu-id="4b1e5-145">Relationships</span></span>
<span data-ttu-id="4b1e5-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b1e5-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b1e5-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b1e5-147">JSON Representation</span></span>
<span data-ttu-id="4b1e5-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b1e5-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
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



