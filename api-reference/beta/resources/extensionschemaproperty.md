---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: keylimesoda
ms.openlocfilehash: e28642e12e7c9bb52b16c21e775e91562de1ebdb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423675"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="0add5-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="0add5-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="0add5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0add5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0add5-105">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="0add5-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="0add5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0add5-106">Properties</span></span>
| <span data-ttu-id="0add5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0add5-107">Property</span></span>     | <span data-ttu-id="0add5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0add5-108">Type</span></span>   |<span data-ttu-id="0add5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0add5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0add5-110">nome</span><span class="sxs-lookup"><span data-stu-id="0add5-110">name</span></span>|<span data-ttu-id="0add5-111">String</span><span class="sxs-lookup"><span data-stu-id="0add5-111">String</span></span>| <span data-ttu-id="0add5-112">O nome da propriedade fortemente tipada definida como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="0add5-112">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="0add5-113">type</span><span class="sxs-lookup"><span data-stu-id="0add5-113">type</span></span>|<span data-ttu-id="0add5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0add5-114">String</span></span>| <span data-ttu-id="0add5-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="0add5-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="0add5-118">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="0add5-118">Supported property data types</span></span> 
<span data-ttu-id="0add5-119">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="0add5-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="0add5-120">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="0add5-120">Property Type</span></span> | <span data-ttu-id="0add5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="0add5-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="0add5-122">Binária</span><span class="sxs-lookup"><span data-stu-id="0add5-122">Binary</span></span> | <span data-ttu-id="0add5-123">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="0add5-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="0add5-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0add5-124">Boolean</span></span> | <span data-ttu-id="0add5-125">Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="0add5-125">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="0add5-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="0add5-126">DateTime</span></span> | <span data-ttu-id="0add5-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="0add5-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="0add5-129">Inteiro</span><span class="sxs-lookup"><span data-stu-id="0add5-129">Integer</span></span> | <span data-ttu-id="0add5-p103">Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="0add5-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="0add5-132">String</span><span class="sxs-lookup"><span data-stu-id="0add5-132">String</span></span> | <span data-ttu-id="0add5-133">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="0add5-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0add5-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0add5-134">JSON representation</span></span>
<span data-ttu-id="0add5-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0add5-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
