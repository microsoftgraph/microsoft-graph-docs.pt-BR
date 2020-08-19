---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
author: keylimesoda
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 623dd4fa92036a3c542bebf791dc802ce0d53520
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812334"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="a549e-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="a549e-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="a549e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a549e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a549e-105">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="a549e-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="a549e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a549e-106">Properties</span></span>
| <span data-ttu-id="a549e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a549e-107">Property</span></span>     | <span data-ttu-id="a549e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a549e-108">Type</span></span>   |<span data-ttu-id="a549e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a549e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a549e-110">nome</span><span class="sxs-lookup"><span data-stu-id="a549e-110">name</span></span>|<span data-ttu-id="a549e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a549e-111">String</span></span>| <span data-ttu-id="a549e-112">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="a549e-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="a549e-113">type</span><span class="sxs-lookup"><span data-stu-id="a549e-113">type</span></span>|<span data-ttu-id="a549e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a549e-114">String</span></span>| <span data-ttu-id="a549e-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="a549e-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="a549e-118">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="a549e-118">Supported property data types</span></span>
<span data-ttu-id="a549e-119">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="a549e-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="a549e-120">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="a549e-120">Property Type</span></span> | <span data-ttu-id="a549e-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a549e-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="a549e-122">Binária</span><span class="sxs-lookup"><span data-stu-id="a549e-122">Binary</span></span> | <span data-ttu-id="a549e-123">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="a549e-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="a549e-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="a549e-124">Boolean</span></span> | <span data-ttu-id="a549e-125">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="a549e-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="a549e-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="a549e-126">DateTime</span></span> | <span data-ttu-id="a549e-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="a549e-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="a549e-129">Inteiro</span><span class="sxs-lookup"><span data-stu-id="a549e-129">Integer</span></span> | <span data-ttu-id="a549e-130">Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="a549e-130">32-bit value.</span></span> <span data-ttu-id="a549e-131">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="a549e-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="a549e-132">String</span><span class="sxs-lookup"><span data-stu-id="a549e-132">String</span></span> | <span data-ttu-id="a549e-133">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a549e-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a549e-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a549e-134">JSON representation</span></span>
<span data-ttu-id="a549e-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a549e-135">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
