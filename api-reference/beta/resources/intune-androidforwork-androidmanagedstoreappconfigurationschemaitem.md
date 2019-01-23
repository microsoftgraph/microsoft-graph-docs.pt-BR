---
title: tipo de recurso de androidManagedStoreAppConfigurationSchemaItem
description: Item de configuração único dentro do esquema de configuração personalizada de um aplicativo Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398916"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="76b36-103">tipo de recurso de androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="76b36-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="76b36-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="76b36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76b36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76b36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76b36-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="76b36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b36-107">Item de configuração único dentro do esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="76b36-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="76b36-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76b36-108">Properties</span></span>
|<span data-ttu-id="76b36-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76b36-109">Property</span></span>|<span data-ttu-id="76b36-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="76b36-110">Type</span></span>|<span data-ttu-id="76b36-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76b36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b36-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="76b36-112">schemaItemKey</span></span>|<span data-ttu-id="76b36-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b36-113">String</span></span>|<span data-ttu-id="76b36-114">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="76b36-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="76b36-115">displayName</span><span class="sxs-lookup"><span data-stu-id="76b36-115">displayName</span></span>|<span data-ttu-id="76b36-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b36-116">String</span></span>|<span data-ttu-id="76b36-117">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="76b36-117">Human readable name</span></span>|
|<span data-ttu-id="76b36-118">description</span><span class="sxs-lookup"><span data-stu-id="76b36-118">description</span></span>|<span data-ttu-id="76b36-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b36-119">String</span></span>|<span data-ttu-id="76b36-120">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="76b36-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="76b36-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="76b36-121">defaultBoolValue</span></span>|<span data-ttu-id="76b36-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="76b36-122">Boolean</span></span>|<span data-ttu-id="76b36-123">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="76b36-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="76b36-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="76b36-124">defaultIntValue</span></span>|<span data-ttu-id="76b36-125">Int32</span><span class="sxs-lookup"><span data-stu-id="76b36-125">Int32</span></span>|<span data-ttu-id="76b36-126">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="76b36-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="76b36-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="76b36-127">defaultStringValue</span></span>|<span data-ttu-id="76b36-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b36-128">String</span></span>|<span data-ttu-id="76b36-129">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="76b36-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="76b36-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="76b36-130">defaultStringArrayValue</span></span>|<span data-ttu-id="76b36-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="76b36-131">String collection</span></span>|<span data-ttu-id="76b36-132">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="76b36-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="76b36-133">dataType</span><span class="sxs-lookup"><span data-stu-id="76b36-133">dataType</span></span>|[<span data-ttu-id="76b36-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="76b36-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="76b36-135">O tipo de valor que descreve este item.</span><span class="sxs-lookup"><span data-stu-id="76b36-135">The type of value this item describes.</span></span> <span data-ttu-id="76b36-136">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="76b36-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="76b36-137">selections</span><span class="sxs-lookup"><span data-stu-id="76b36-137">selections</span></span>|<span data-ttu-id="76b36-138">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="76b36-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="76b36-139">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="76b36-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="76b36-140">Relações</span><span class="sxs-lookup"><span data-stu-id="76b36-140">Relationships</span></span>
<span data-ttu-id="76b36-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76b36-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76b36-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76b36-142">JSON Representation</span></span>
<span data-ttu-id="76b36-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76b36-143">Here is a JSON representation of the resource.</span></span>
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




