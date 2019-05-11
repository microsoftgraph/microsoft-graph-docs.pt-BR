---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3012542315cd30a565da315a9d383757557b1008
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950540"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="26340-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="26340-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="26340-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26340-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26340-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26340-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26340-106">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="26340-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="26340-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26340-107">Properties</span></span>
|<span data-ttu-id="26340-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26340-108">Property</span></span>|<span data-ttu-id="26340-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="26340-109">Type</span></span>|<span data-ttu-id="26340-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26340-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26340-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="26340-111">schemaItemKey</span></span>|<span data-ttu-id="26340-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26340-112">String</span></span>|<span data-ttu-id="26340-113">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="26340-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="26340-114">displayName</span><span class="sxs-lookup"><span data-stu-id="26340-114">displayName</span></span>|<span data-ttu-id="26340-115">String</span><span class="sxs-lookup"><span data-stu-id="26340-115">String</span></span>|<span data-ttu-id="26340-116">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="26340-116">Human readable name</span></span>|
|<span data-ttu-id="26340-117">description</span><span class="sxs-lookup"><span data-stu-id="26340-117">description</span></span>|<span data-ttu-id="26340-118">String</span><span class="sxs-lookup"><span data-stu-id="26340-118">String</span></span>|<span data-ttu-id="26340-119">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26340-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="26340-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="26340-120">defaultBoolValue</span></span>|<span data-ttu-id="26340-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="26340-121">Boolean</span></span>|<span data-ttu-id="26340-122">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26340-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="26340-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="26340-123">defaultIntValue</span></span>|<span data-ttu-id="26340-124">Int32</span><span class="sxs-lookup"><span data-stu-id="26340-124">Int32</span></span>|<span data-ttu-id="26340-125">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26340-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="26340-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="26340-126">defaultStringValue</span></span>|<span data-ttu-id="26340-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26340-127">String</span></span>|<span data-ttu-id="26340-128">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26340-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="26340-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="26340-129">defaultStringArrayValue</span></span>|<span data-ttu-id="26340-130">Coleção String</span><span class="sxs-lookup"><span data-stu-id="26340-130">String collection</span></span>|<span data-ttu-id="26340-131">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26340-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="26340-132">dataType</span><span class="sxs-lookup"><span data-stu-id="26340-132">dataType</span></span>|[<span data-ttu-id="26340-133">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="26340-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="26340-134">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="26340-134">The type of value this item describes.</span></span> <span data-ttu-id="26340-135">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="26340-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="26340-136">selections</span><span class="sxs-lookup"><span data-stu-id="26340-136">selections</span></span>|<span data-ttu-id="26340-137">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="26340-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="26340-138">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="26340-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="26340-139">Relações</span><span class="sxs-lookup"><span data-stu-id="26340-139">Relationships</span></span>
<span data-ttu-id="26340-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26340-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26340-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26340-141">JSON Representation</span></span>
<span data-ttu-id="26340-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26340-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




