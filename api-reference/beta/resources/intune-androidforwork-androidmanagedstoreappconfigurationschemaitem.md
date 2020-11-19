---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ebb70d14a608d76acf5bccb3ab4248ca38346e5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269802"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="9ae68-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="9ae68-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="9ae68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ae68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ae68-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ae68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ae68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ae68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ae68-107">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="9ae68-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="9ae68-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ae68-108">Properties</span></span>
|<span data-ttu-id="9ae68-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ae68-109">Property</span></span>|<span data-ttu-id="9ae68-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ae68-110">Type</span></span>|<span data-ttu-id="9ae68-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae68-112">índice</span><span class="sxs-lookup"><span data-stu-id="9ae68-112">index</span></span>|<span data-ttu-id="9ae68-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae68-113">Int32</span></span>|<span data-ttu-id="9ae68-114">Índice exclusivo que o aplicativo usa para manter itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="9ae68-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="9ae68-115">parentIndex</span><span class="sxs-lookup"><span data-stu-id="9ae68-115">parentIndex</span></span>|<span data-ttu-id="9ae68-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae68-116">Int32</span></span>|<span data-ttu-id="9ae68-117">Índice do item de esquema pai para rastrear itens de esquema aninhados</span><span class="sxs-lookup"><span data-stu-id="9ae68-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="9ae68-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="9ae68-118">schemaItemKey</span></span>|<span data-ttu-id="9ae68-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ae68-119">String</span></span>|<span data-ttu-id="9ae68-120">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="9ae68-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="9ae68-121">displayName</span><span class="sxs-lookup"><span data-stu-id="9ae68-121">displayName</span></span>|<span data-ttu-id="9ae68-122">String</span><span class="sxs-lookup"><span data-stu-id="9ae68-122">String</span></span>|<span data-ttu-id="9ae68-123">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="9ae68-123">Human readable name</span></span>|
|<span data-ttu-id="9ae68-124">description</span><span class="sxs-lookup"><span data-stu-id="9ae68-124">description</span></span>|<span data-ttu-id="9ae68-125">String</span><span class="sxs-lookup"><span data-stu-id="9ae68-125">String</span></span>|<span data-ttu-id="9ae68-126">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae68-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="9ae68-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="9ae68-127">defaultBoolValue</span></span>|<span data-ttu-id="9ae68-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ae68-128">Boolean</span></span>|<span data-ttu-id="9ae68-129">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae68-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9ae68-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="9ae68-130">defaultIntValue</span></span>|<span data-ttu-id="9ae68-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae68-131">Int32</span></span>|<span data-ttu-id="9ae68-132">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae68-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9ae68-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="9ae68-133">defaultStringValue</span></span>|<span data-ttu-id="9ae68-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ae68-134">String</span></span>|<span data-ttu-id="9ae68-135">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae68-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9ae68-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="9ae68-136">defaultStringArrayValue</span></span>|<span data-ttu-id="9ae68-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9ae68-137">String collection</span></span>|<span data-ttu-id="9ae68-138">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae68-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9ae68-139">dataType</span><span class="sxs-lookup"><span data-stu-id="9ae68-139">dataType</span></span>|[<span data-ttu-id="9ae68-140">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="9ae68-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="9ae68-141">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="9ae68-141">The type of value this item describes.</span></span> <span data-ttu-id="9ae68-142">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="9ae68-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="9ae68-143">selections</span><span class="sxs-lookup"><span data-stu-id="9ae68-143">selections</span></span>|<span data-ttu-id="9ae68-144">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9ae68-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9ae68-145">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="9ae68-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ae68-146">Relações</span><span class="sxs-lookup"><span data-stu-id="9ae68-146">Relationships</span></span>
<span data-ttu-id="9ae68-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ae68-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ae68-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ae68-148">JSON Representation</span></span>
<span data-ttu-id="9ae68-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ae68-149">Here is a JSON representation of the resource.</span></span>
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




