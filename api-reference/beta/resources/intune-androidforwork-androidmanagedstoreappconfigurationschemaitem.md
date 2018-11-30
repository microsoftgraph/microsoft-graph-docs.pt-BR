---
title: tipo de recurso de androidManagedStoreAppConfigurationSchemaItem
description: Item de configuração único dentro do esquema de configuração personalizada de um aplicativo Android.
ms.openlocfilehash: 94ae8735800e4f79be2e7c61f8b971bafd8c394f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039227"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="7fc00-103">tipo de recurso de androidManagedStoreAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="7fc00-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="7fc00-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fc00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fc00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fc00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fc00-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fc00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fc00-107">Item de configuração único dentro do esquema de configuração personalizada de um aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="7fc00-107">Single configuration item inside an Android application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="7fc00-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fc00-108">Properties</span></span>
|<span data-ttu-id="7fc00-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fc00-109">Property</span></span>|<span data-ttu-id="7fc00-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fc00-110">Type</span></span>|<span data-ttu-id="7fc00-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fc00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc00-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="7fc00-112">schemaItemKey</span></span>|<span data-ttu-id="7fc00-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fc00-113">String</span></span>|<span data-ttu-id="7fc00-114">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="7fc00-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="7fc00-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7fc00-115">displayName</span></span>|<span data-ttu-id="7fc00-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fc00-116">String</span></span>|<span data-ttu-id="7fc00-117">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="7fc00-117">Human readable name</span></span>|
|<span data-ttu-id="7fc00-118">description</span><span class="sxs-lookup"><span data-stu-id="7fc00-118">description</span></span>|<span data-ttu-id="7fc00-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fc00-119">String</span></span>|<span data-ttu-id="7fc00-120">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc00-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="7fc00-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="7fc00-121">defaultBoolValue</span></span>|<span data-ttu-id="7fc00-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7fc00-122">Boolean</span></span>|<span data-ttu-id="7fc00-123">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc00-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7fc00-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="7fc00-124">defaultIntValue</span></span>|<span data-ttu-id="7fc00-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7fc00-125">Int32</span></span>|<span data-ttu-id="7fc00-126">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc00-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7fc00-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="7fc00-127">defaultStringValue</span></span>|<span data-ttu-id="7fc00-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fc00-128">String</span></span>|<span data-ttu-id="7fc00-129">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc00-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7fc00-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="7fc00-130">defaultStringArrayValue</span></span>|<span data-ttu-id="7fc00-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7fc00-131">String collection</span></span>|<span data-ttu-id="7fc00-132">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc00-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="7fc00-133">dataType</span><span class="sxs-lookup"><span data-stu-id="7fc00-133">dataType</span></span>|[<span data-ttu-id="7fc00-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="7fc00-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="7fc00-135">O tipo de valor que descreve este item.</span><span class="sxs-lookup"><span data-stu-id="7fc00-135">The type of value this item describes.</span></span> <span data-ttu-id="7fc00-136">Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="7fc00-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="7fc00-137">selections</span><span class="sxs-lookup"><span data-stu-id="7fc00-137">selections</span></span>|<span data-ttu-id="7fc00-138">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7fc00-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fc00-139">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="7fc00-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fc00-140">Relações</span><span class="sxs-lookup"><span data-stu-id="7fc00-140">Relationships</span></span>
<span data-ttu-id="7fc00-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fc00-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fc00-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fc00-142">JSON Representation</span></span>
<span data-ttu-id="7fc00-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fc00-143">Here is a JSON representation of the resource.</span></span>
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





