---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3313ba3cef3a996d030d25ac1bb24492b28b4b2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950771"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="c8541-103">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="c8541-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="c8541-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8541-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8541-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8541-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8541-106">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="c8541-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="c8541-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8541-107">Properties</span></span>
|<span data-ttu-id="c8541-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8541-108">Property</span></span>|<span data-ttu-id="c8541-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8541-109">Type</span></span>|<span data-ttu-id="c8541-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8541-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8541-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="c8541-111">schemaItemKey</span></span>|<span data-ttu-id="c8541-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8541-112">String</span></span>|<span data-ttu-id="c8541-113">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="c8541-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="c8541-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c8541-114">displayName</span></span>|<span data-ttu-id="c8541-115">String</span><span class="sxs-lookup"><span data-stu-id="c8541-115">String</span></span>|<span data-ttu-id="c8541-116">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="c8541-116">Human readable name</span></span>|
|<span data-ttu-id="c8541-117">description</span><span class="sxs-lookup"><span data-stu-id="c8541-117">description</span></span>|<span data-ttu-id="c8541-118">String</span><span class="sxs-lookup"><span data-stu-id="c8541-118">String</span></span>|<span data-ttu-id="c8541-119">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8541-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="c8541-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="c8541-120">defaultBoolValue</span></span>|<span data-ttu-id="c8541-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8541-121">Boolean</span></span>|<span data-ttu-id="c8541-122">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8541-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c8541-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="c8541-123">defaultIntValue</span></span>|<span data-ttu-id="c8541-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c8541-124">Int32</span></span>|<span data-ttu-id="c8541-125">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8541-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c8541-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="c8541-126">defaultStringValue</span></span>|<span data-ttu-id="c8541-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8541-127">String</span></span>|<span data-ttu-id="c8541-128">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8541-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c8541-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="c8541-129">defaultStringArrayValue</span></span>|<span data-ttu-id="c8541-130">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c8541-130">String collection</span></span>|<span data-ttu-id="c8541-131">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8541-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c8541-132">dataType</span><span class="sxs-lookup"><span data-stu-id="c8541-132">dataType</span></span>|[<span data-ttu-id="c8541-133">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="c8541-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="c8541-134">O tipo de valor que este item descreve.</span><span class="sxs-lookup"><span data-stu-id="c8541-134">The type of value this item describes.</span></span> <span data-ttu-id="c8541-135">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="c8541-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="c8541-136">selections</span><span class="sxs-lookup"><span data-stu-id="c8541-136">selections</span></span>|<span data-ttu-id="c8541-137">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c8541-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c8541-138">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="c8541-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8541-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c8541-139">Relationships</span></span>
<span data-ttu-id="c8541-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8541-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8541-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8541-141">JSON Representation</span></span>
<span data-ttu-id="c8541-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8541-142">Here is a JSON representation of the resource.</span></span>
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




