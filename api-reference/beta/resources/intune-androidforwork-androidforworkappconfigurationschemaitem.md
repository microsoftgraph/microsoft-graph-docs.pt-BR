---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0de75506419ea0e403c7f55af07459514abb408c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147730"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="6b403-103">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="6b403-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="6b403-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b403-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b403-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b403-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b403-106">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="6b403-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="6b403-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b403-107">Properties</span></span>
|<span data-ttu-id="6b403-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b403-108">Property</span></span>|<span data-ttu-id="6b403-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b403-109">Type</span></span>|<span data-ttu-id="6b403-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b403-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b403-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="6b403-111">schemaItemKey</span></span>|<span data-ttu-id="6b403-112">String</span><span class="sxs-lookup"><span data-stu-id="6b403-112">String</span></span>|<span data-ttu-id="6b403-113">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="6b403-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="6b403-114">displayName</span><span class="sxs-lookup"><span data-stu-id="6b403-114">displayName</span></span>|<span data-ttu-id="6b403-115">String</span><span class="sxs-lookup"><span data-stu-id="6b403-115">String</span></span>|<span data-ttu-id="6b403-116">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="6b403-116">Human readable name</span></span>|
|<span data-ttu-id="6b403-117">description</span><span class="sxs-lookup"><span data-stu-id="6b403-117">description</span></span>|<span data-ttu-id="6b403-118">String</span><span class="sxs-lookup"><span data-stu-id="6b403-118">String</span></span>|<span data-ttu-id="6b403-119">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b403-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="6b403-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="6b403-120">defaultBoolValue</span></span>|<span data-ttu-id="6b403-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b403-121">Boolean</span></span>|<span data-ttu-id="6b403-122">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b403-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6b403-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="6b403-123">defaultIntValue</span></span>|<span data-ttu-id="6b403-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6b403-124">Int32</span></span>|<span data-ttu-id="6b403-125">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b403-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6b403-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="6b403-126">defaultStringValue</span></span>|<span data-ttu-id="6b403-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b403-127">String</span></span>|<span data-ttu-id="6b403-128">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b403-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6b403-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="6b403-129">defaultStringArrayValue</span></span>|<span data-ttu-id="6b403-130">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6b403-130">String collection</span></span>|<span data-ttu-id="6b403-131">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b403-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="6b403-132">dataType</span><span class="sxs-lookup"><span data-stu-id="6b403-132">dataType</span></span>|[<span data-ttu-id="6b403-133">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="6b403-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="6b403-134">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="6b403-134">The type of value this item describes.</span></span> <span data-ttu-id="6b403-135">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="6b403-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="6b403-136">selections</span><span class="sxs-lookup"><span data-stu-id="6b403-136">selections</span></span>|<span data-ttu-id="6b403-137">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6b403-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6b403-138">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="6b403-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b403-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6b403-139">Relationships</span></span>
<span data-ttu-id="6b403-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b403-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b403-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b403-141">JSON Representation</span></span>
<span data-ttu-id="6b403-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b403-142">Here is a JSON representation of the resource.</span></span>
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




