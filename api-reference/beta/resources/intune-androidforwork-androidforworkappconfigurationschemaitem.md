---
title: Tipo de recurso androidForWorkAppConfigurationSchemaItem
description: Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45370a7c5bec72e63d25e2c8242ac8b07c4cc4e4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392728"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="7d999-103">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="7d999-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="7d999-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d999-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d999-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d999-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d999-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7d999-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d999-107">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="7d999-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="7d999-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d999-108">Properties</span></span>
|<span data-ttu-id="7d999-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d999-109">Property</span></span>|<span data-ttu-id="7d999-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d999-110">Type</span></span>|<span data-ttu-id="7d999-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d999-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d999-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="7d999-112">schemaItemKey</span></span>|<span data-ttu-id="7d999-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d999-113">String</span></span>|<span data-ttu-id="7d999-114">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="7d999-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="7d999-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7d999-115">displayName</span></span>|<span data-ttu-id="7d999-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d999-116">String</span></span>|<span data-ttu-id="7d999-117">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="7d999-117">Human readable name</span></span>|
|<span data-ttu-id="7d999-118">description</span><span class="sxs-lookup"><span data-stu-id="7d999-118">description</span></span>|<span data-ttu-id="7d999-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d999-119">String</span></span>|<span data-ttu-id="7d999-120">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d999-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="7d999-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="7d999-121">defaultBoolValue</span></span>|<span data-ttu-id="7d999-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d999-122">Boolean</span></span>|<span data-ttu-id="7d999-123">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d999-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7d999-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="7d999-124">defaultIntValue</span></span>|<span data-ttu-id="7d999-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7d999-125">Int32</span></span>|<span data-ttu-id="7d999-126">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d999-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7d999-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="7d999-127">defaultStringValue</span></span>|<span data-ttu-id="7d999-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d999-128">String</span></span>|<span data-ttu-id="7d999-129">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d999-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7d999-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="7d999-130">defaultStringArrayValue</span></span>|<span data-ttu-id="7d999-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7d999-131">String collection</span></span>|<span data-ttu-id="7d999-132">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d999-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7d999-133">dataType</span><span class="sxs-lookup"><span data-stu-id="7d999-133">dataType</span></span>|[<span data-ttu-id="7d999-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="7d999-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="7d999-135">O tipo de valor que descreve este item.</span><span class="sxs-lookup"><span data-stu-id="7d999-135">The type of value this item describes.</span></span> <span data-ttu-id="7d999-136">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="7d999-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="7d999-137">selections</span><span class="sxs-lookup"><span data-stu-id="7d999-137">selections</span></span>|<span data-ttu-id="7d999-138">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7d999-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7d999-139">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="7d999-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d999-140">Relações</span><span class="sxs-lookup"><span data-stu-id="7d999-140">Relationships</span></span>
<span data-ttu-id="7d999-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d999-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d999-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d999-142">JSON Representation</span></span>
<span data-ttu-id="7d999-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d999-143">Here is a JSON representation of the resource.</span></span>
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




