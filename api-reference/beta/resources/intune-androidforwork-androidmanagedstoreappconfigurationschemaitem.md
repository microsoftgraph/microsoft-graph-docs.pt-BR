---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 744715e3169dd0b6b7aa4fa9a7fd9be1f341720f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467872"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="015c9-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="015c9-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="015c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="015c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="015c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="015c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="015c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="015c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="015c9-107">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="015c9-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="015c9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="015c9-108">Properties</span></span>
|<span data-ttu-id="015c9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="015c9-109">Property</span></span>|<span data-ttu-id="015c9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="015c9-110">Type</span></span>|<span data-ttu-id="015c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="015c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="015c9-112">índice</span><span class="sxs-lookup"><span data-stu-id="015c9-112">index</span></span>|<span data-ttu-id="015c9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="015c9-113">Int32</span></span>|<span data-ttu-id="015c9-114">Índice exclusivo que o aplicativo usa para manter itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="015c9-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="015c9-115">parentIndex</span><span class="sxs-lookup"><span data-stu-id="015c9-115">parentIndex</span></span>|<span data-ttu-id="015c9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="015c9-116">Int32</span></span>|<span data-ttu-id="015c9-117">Índice do item de esquema pai para rastrear itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="015c9-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="015c9-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="015c9-118">schemaItemKey</span></span>|<span data-ttu-id="015c9-119">String</span><span class="sxs-lookup"><span data-stu-id="015c9-119">String</span></span>|<span data-ttu-id="015c9-120">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="015c9-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="015c9-121">displayName</span><span class="sxs-lookup"><span data-stu-id="015c9-121">displayName</span></span>|<span data-ttu-id="015c9-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="015c9-122">String</span></span>|<span data-ttu-id="015c9-123">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="015c9-123">Human readable name</span></span>|
|<span data-ttu-id="015c9-124">description</span><span class="sxs-lookup"><span data-stu-id="015c9-124">description</span></span>|<span data-ttu-id="015c9-125">String</span><span class="sxs-lookup"><span data-stu-id="015c9-125">String</span></span>|<span data-ttu-id="015c9-126">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="015c9-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="015c9-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="015c9-127">defaultBoolValue</span></span>|<span data-ttu-id="015c9-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="015c9-128">Boolean</span></span>|<span data-ttu-id="015c9-129">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="015c9-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="015c9-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="015c9-130">defaultIntValue</span></span>|<span data-ttu-id="015c9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="015c9-131">Int32</span></span>|<span data-ttu-id="015c9-132">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="015c9-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="015c9-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="015c9-133">defaultStringValue</span></span>|<span data-ttu-id="015c9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="015c9-134">String</span></span>|<span data-ttu-id="015c9-135">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="015c9-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="015c9-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="015c9-136">defaultStringArrayValue</span></span>|<span data-ttu-id="015c9-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="015c9-137">String collection</span></span>|<span data-ttu-id="015c9-138">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="015c9-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="015c9-139">dataType</span><span class="sxs-lookup"><span data-stu-id="015c9-139">dataType</span></span>|[<span data-ttu-id="015c9-140">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="015c9-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="015c9-141">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="015c9-141">The type of value this item describes.</span></span> <span data-ttu-id="015c9-142">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="015c9-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="015c9-143">selections</span><span class="sxs-lookup"><span data-stu-id="015c9-143">selections</span></span>|<span data-ttu-id="015c9-144">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="015c9-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="015c9-145">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="015c9-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="015c9-146">Relações</span><span class="sxs-lookup"><span data-stu-id="015c9-146">Relationships</span></span>
<span data-ttu-id="015c9-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="015c9-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="015c9-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="015c9-148">JSON Representation</span></span>
<span data-ttu-id="015c9-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="015c9-149">Here is a JSON representation of the resource.</span></span>
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



