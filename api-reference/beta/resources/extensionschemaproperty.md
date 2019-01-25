---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
ms.openlocfilehash: bb044aa2f85ea5accdba4ed43a1a5b1c856a209d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511503"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="d74f9-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="d74f9-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d74f9-104">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="d74f9-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="d74f9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d74f9-105">Properties</span></span>
| <span data-ttu-id="d74f9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d74f9-106">Property</span></span>     | <span data-ttu-id="d74f9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d74f9-107">Type</span></span>   |<span data-ttu-id="d74f9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d74f9-109">name</span><span class="sxs-lookup"><span data-stu-id="d74f9-109">name</span></span>|<span data-ttu-id="d74f9-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d74f9-110">String</span></span>| <span data-ttu-id="d74f9-111">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="d74f9-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="d74f9-112">type</span><span class="sxs-lookup"><span data-stu-id="d74f9-112">type</span></span>|<span data-ttu-id="d74f9-113">String</span><span class="sxs-lookup"><span data-stu-id="d74f9-113">String</span></span>| <span data-ttu-id="d74f9-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="d74f9-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="d74f9-117">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="d74f9-117">Supported property data types</span></span> 
<span data-ttu-id="d74f9-118">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="d74f9-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="d74f9-119">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="d74f9-119">Property Type</span></span> | <span data-ttu-id="d74f9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d74f9-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="d74f9-121">Binária</span><span class="sxs-lookup"><span data-stu-id="d74f9-121">Binary</span></span> | <span data-ttu-id="d74f9-122">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="d74f9-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="d74f9-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="d74f9-123">Boolean</span></span> | <span data-ttu-id="d74f9-124">Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="d74f9-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="d74f9-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="d74f9-125">DateTime</span></span> | <span data-ttu-id="d74f9-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="d74f9-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="d74f9-128">Inteiro</span><span class="sxs-lookup"><span data-stu-id="d74f9-128">Integer</span></span> | <span data-ttu-id="d74f9-p103">Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="d74f9-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="d74f9-131">String</span><span class="sxs-lookup"><span data-stu-id="d74f9-131">String</span></span> | <span data-ttu-id="d74f9-132">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d74f9-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d74f9-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d74f9-133">JSON representation</span></span>
<span data-ttu-id="d74f9-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d74f9-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/extensionschemaproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
