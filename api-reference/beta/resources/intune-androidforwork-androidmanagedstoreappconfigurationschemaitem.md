---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99a77dccc7bec8e4d28944ac9d5e5af16a98b462
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019688"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="e3a27-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="e3a27-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="e3a27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3a27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3a27-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3a27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3a27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3a27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3a27-107">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="e3a27-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="e3a27-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3a27-108">Properties</span></span>
|<span data-ttu-id="e3a27-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3a27-109">Property</span></span>|<span data-ttu-id="e3a27-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3a27-110">Type</span></span>|<span data-ttu-id="e3a27-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3a27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a27-112">índice</span><span class="sxs-lookup"><span data-stu-id="e3a27-112">index</span></span>|<span data-ttu-id="e3a27-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a27-113">Int32</span></span>|<span data-ttu-id="e3a27-114">Índice exclusivo que o aplicativo usa para manter itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="e3a27-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="e3a27-115">parentIndex</span><span class="sxs-lookup"><span data-stu-id="e3a27-115">parentIndex</span></span>|<span data-ttu-id="e3a27-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a27-116">Int32</span></span>|<span data-ttu-id="e3a27-117">Índice do item de esquema pai para rastrear itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="e3a27-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="e3a27-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="e3a27-118">schemaItemKey</span></span>|<span data-ttu-id="e3a27-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3a27-119">String</span></span>|<span data-ttu-id="e3a27-120">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="e3a27-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="e3a27-121">displayName</span><span class="sxs-lookup"><span data-stu-id="e3a27-121">displayName</span></span>|<span data-ttu-id="e3a27-122">String</span><span class="sxs-lookup"><span data-stu-id="e3a27-122">String</span></span>|<span data-ttu-id="e3a27-123">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="e3a27-123">Human readable name</span></span>|
|<span data-ttu-id="e3a27-124">description</span><span class="sxs-lookup"><span data-stu-id="e3a27-124">description</span></span>|<span data-ttu-id="e3a27-125">String</span><span class="sxs-lookup"><span data-stu-id="e3a27-125">String</span></span>|<span data-ttu-id="e3a27-126">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3a27-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="e3a27-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="e3a27-127">defaultBoolValue</span></span>|<span data-ttu-id="e3a27-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3a27-128">Boolean</span></span>|<span data-ttu-id="e3a27-129">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3a27-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e3a27-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="e3a27-130">defaultIntValue</span></span>|<span data-ttu-id="e3a27-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a27-131">Int32</span></span>|<span data-ttu-id="e3a27-132">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3a27-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e3a27-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="e3a27-133">defaultStringValue</span></span>|<span data-ttu-id="e3a27-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3a27-134">String</span></span>|<span data-ttu-id="e3a27-135">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3a27-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e3a27-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="e3a27-136">defaultStringArrayValue</span></span>|<span data-ttu-id="e3a27-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e3a27-137">String collection</span></span>|<span data-ttu-id="e3a27-138">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3a27-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e3a27-139">dataType</span><span class="sxs-lookup"><span data-stu-id="e3a27-139">dataType</span></span>|[<span data-ttu-id="e3a27-140">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="e3a27-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="e3a27-141">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="e3a27-141">The type of value this item describes.</span></span> <span data-ttu-id="e3a27-142">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="e3a27-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="e3a27-143">selections</span><span class="sxs-lookup"><span data-stu-id="e3a27-143">selections</span></span>|<span data-ttu-id="e3a27-144">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e3a27-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e3a27-145">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="e3a27-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3a27-146">Relações</span><span class="sxs-lookup"><span data-stu-id="e3a27-146">Relationships</span></span>
<span data-ttu-id="e3a27-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3a27-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3a27-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3a27-148">JSON Representation</span></span>
<span data-ttu-id="e3a27-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3a27-149">Here is a JSON representation of the resource.</span></span>
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






