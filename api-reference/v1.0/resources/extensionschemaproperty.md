---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a684d71aa25267c1b2f19f13d35d796825783544
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531452"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="66b5f-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="66b5f-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="66b5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66b5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66b5f-105">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="66b5f-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="66b5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66b5f-106">Properties</span></span>
| <span data-ttu-id="66b5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66b5f-107">Property</span></span>     | <span data-ttu-id="66b5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="66b5f-108">Type</span></span>   |<span data-ttu-id="66b5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66b5f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66b5f-110">nome</span><span class="sxs-lookup"><span data-stu-id="66b5f-110">name</span></span>|<span data-ttu-id="66b5f-111">String</span><span class="sxs-lookup"><span data-stu-id="66b5f-111">String</span></span>| <span data-ttu-id="66b5f-112">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="66b5f-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="66b5f-113">type</span><span class="sxs-lookup"><span data-stu-id="66b5f-113">type</span></span>|<span data-ttu-id="66b5f-114">String</span><span class="sxs-lookup"><span data-stu-id="66b5f-114">String</span></span>| <span data-ttu-id="66b5f-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="66b5f-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="66b5f-118">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="66b5f-118">Supported property data types</span></span> 
<span data-ttu-id="66b5f-119">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="66b5f-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="66b5f-120">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="66b5f-120">Property Type</span></span> | <span data-ttu-id="66b5f-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="66b5f-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="66b5f-122">Binária</span><span class="sxs-lookup"><span data-stu-id="66b5f-122">Binary</span></span> | <span data-ttu-id="66b5f-123">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="66b5f-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="66b5f-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="66b5f-124">Boolean</span></span> | <span data-ttu-id="66b5f-125">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="66b5f-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="66b5f-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="66b5f-126">DateTime</span></span> | <span data-ttu-id="66b5f-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="66b5f-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="66b5f-129">Inteiro</span><span class="sxs-lookup"><span data-stu-id="66b5f-129">Integer</span></span> | <span data-ttu-id="66b5f-130">Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="66b5f-130">32-bit value.</span></span> <span data-ttu-id="66b5f-131">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="66b5f-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="66b5f-132">String</span><span class="sxs-lookup"><span data-stu-id="66b5f-132">String</span></span> | <span data-ttu-id="66b5f-133">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="66b5f-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66b5f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66b5f-134">JSON representation</span></span>
<span data-ttu-id="66b5f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66b5f-135">Here is a JSON representation of the resource.</span></span>

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
