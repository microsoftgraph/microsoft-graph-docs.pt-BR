---
title: tipo de recurso androidManagedStoreAppConfigurationSchemaItem
description: Único item de configuração no esquema de configuração personalizada de um aplicativo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964916f9f6a46cd8b276e304bfb341d6504db0d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552431"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="81d39-103">tipo de recurso androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="81d39-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="81d39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81d39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81d39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81d39-106">Único item de configuração no esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="81d39-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="81d39-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81d39-107">Properties</span></span>
|<span data-ttu-id="81d39-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81d39-108">Property</span></span>|<span data-ttu-id="81d39-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81d39-109">Type</span></span>|<span data-ttu-id="81d39-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81d39-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d39-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="81d39-111">schemaItemKey</span></span>|<span data-ttu-id="81d39-112">String</span><span class="sxs-lookup"><span data-stu-id="81d39-112">String</span></span>|<span data-ttu-id="81d39-113">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="81d39-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="81d39-114">displayName</span><span class="sxs-lookup"><span data-stu-id="81d39-114">displayName</span></span>|<span data-ttu-id="81d39-115">String</span><span class="sxs-lookup"><span data-stu-id="81d39-115">String</span></span>|<span data-ttu-id="81d39-116">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="81d39-116">Human readable name</span></span>|
|<span data-ttu-id="81d39-117">description</span><span class="sxs-lookup"><span data-stu-id="81d39-117">description</span></span>|<span data-ttu-id="81d39-118">String</span><span class="sxs-lookup"><span data-stu-id="81d39-118">String</span></span>|<span data-ttu-id="81d39-119">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d39-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="81d39-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="81d39-120">defaultBoolValue</span></span>|<span data-ttu-id="81d39-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d39-121">Boolean</span></span>|<span data-ttu-id="81d39-122">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d39-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="81d39-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="81d39-123">defaultIntValue</span></span>|<span data-ttu-id="81d39-124">Int32</span><span class="sxs-lookup"><span data-stu-id="81d39-124">Int32</span></span>|<span data-ttu-id="81d39-125">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d39-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="81d39-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="81d39-126">defaultStringValue</span></span>|<span data-ttu-id="81d39-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81d39-127">String</span></span>|<span data-ttu-id="81d39-128">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d39-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="81d39-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="81d39-129">defaultStringArrayValue</span></span>|<span data-ttu-id="81d39-130">Coleção String</span><span class="sxs-lookup"><span data-stu-id="81d39-130">String collection</span></span>|<span data-ttu-id="81d39-131">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d39-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="81d39-132">dataType</span><span class="sxs-lookup"><span data-stu-id="81d39-132">dataType</span></span>|[<span data-ttu-id="81d39-133">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="81d39-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="81d39-134">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="81d39-134">The type of value this item describes.</span></span> <span data-ttu-id="81d39-135">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="81d39-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="81d39-136">selections</span><span class="sxs-lookup"><span data-stu-id="81d39-136">selections</span></span>|<span data-ttu-id="81d39-137">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="81d39-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81d39-138">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="81d39-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="81d39-139">Relações</span><span class="sxs-lookup"><span data-stu-id="81d39-139">Relationships</span></span>
<span data-ttu-id="81d39-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81d39-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81d39-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81d39-141">JSON Representation</span></span>
<span data-ttu-id="81d39-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81d39-142">Here is a JSON representation of the resource.</span></span>
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





