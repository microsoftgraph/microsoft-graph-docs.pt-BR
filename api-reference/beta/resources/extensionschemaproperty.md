---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d36cf90e82e0240842fd9631e2471f9ee834fcb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972058"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="d6222-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="d6222-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6222-104">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="d6222-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="d6222-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6222-105">Properties</span></span>
| <span data-ttu-id="d6222-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6222-106">Property</span></span>     | <span data-ttu-id="d6222-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6222-107">Type</span></span>   |<span data-ttu-id="d6222-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6222-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6222-109">name</span><span class="sxs-lookup"><span data-stu-id="d6222-109">name</span></span>|<span data-ttu-id="d6222-110">String</span><span class="sxs-lookup"><span data-stu-id="d6222-110">String</span></span>| <span data-ttu-id="d6222-111">O nome da propriedade fortemente tipada definida como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="d6222-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="d6222-112">type</span><span class="sxs-lookup"><span data-stu-id="d6222-112">type</span></span>|<span data-ttu-id="d6222-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6222-113">String</span></span>| <span data-ttu-id="d6222-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="d6222-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="d6222-117">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="d6222-117">Supported property data types</span></span> 
<span data-ttu-id="d6222-118">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="d6222-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="d6222-119">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="d6222-119">Property Type</span></span> | <span data-ttu-id="d6222-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6222-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="d6222-121">Binária</span><span class="sxs-lookup"><span data-stu-id="d6222-121">Binary</span></span> | <span data-ttu-id="d6222-122">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="d6222-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="d6222-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6222-123">Boolean</span></span> | <span data-ttu-id="d6222-124">Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="d6222-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="d6222-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="d6222-125">DateTime</span></span> | <span data-ttu-id="d6222-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="d6222-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="d6222-128">Inteiro</span><span class="sxs-lookup"><span data-stu-id="d6222-128">Integer</span></span> | <span data-ttu-id="d6222-p103">Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="d6222-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="d6222-131">String</span><span class="sxs-lookup"><span data-stu-id="d6222-131">String</span></span> | <span data-ttu-id="d6222-132">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d6222-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6222-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6222-133">JSON representation</span></span>
<span data-ttu-id="d6222-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6222-134">Here is a JSON representation of the resource.</span></span>

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
