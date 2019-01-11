---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
ms.openlocfilehash: 384f60c323ca6c6fb23d2f4811a6d2cb918bf844
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880567"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="55897-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="55897-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="55897-104">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="55897-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="55897-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55897-105">Properties</span></span>
| <span data-ttu-id="55897-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55897-106">Property</span></span>     | <span data-ttu-id="55897-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="55897-107">Type</span></span>   |<span data-ttu-id="55897-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="55897-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55897-109">name</span><span class="sxs-lookup"><span data-stu-id="55897-109">name</span></span>|<span data-ttu-id="55897-110">String</span><span class="sxs-lookup"><span data-stu-id="55897-110">String</span></span>| <span data-ttu-id="55897-111">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="55897-111">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="55897-112">type</span><span class="sxs-lookup"><span data-stu-id="55897-112">type</span></span>|<span data-ttu-id="55897-113">String</span><span class="sxs-lookup"><span data-stu-id="55897-113">String</span></span>| <span data-ttu-id="55897-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="55897-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="55897-117">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="55897-117">Supported property data types</span></span> 
<span data-ttu-id="55897-118">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="55897-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="55897-119">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="55897-119">Property Type</span></span> | <span data-ttu-id="55897-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="55897-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="55897-121">Binária</span><span class="sxs-lookup"><span data-stu-id="55897-121">Binary</span></span> | <span data-ttu-id="55897-122">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="55897-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="55897-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="55897-123">Boolean</span></span> | <span data-ttu-id="55897-124">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="55897-124">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="55897-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="55897-125">DateTime</span></span> | <span data-ttu-id="55897-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="55897-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="55897-128">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="55897-128">Integer</span></span> | <span data-ttu-id="55897-129">Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="55897-129">32-bit value.</span></span> <span data-ttu-id="55897-130">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="55897-130">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="55897-131">String</span><span class="sxs-lookup"><span data-stu-id="55897-131">String</span></span> | <span data-ttu-id="55897-132">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="55897-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="55897-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55897-133">JSON representation</span></span>
<span data-ttu-id="55897-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55897-134">Here is a JSON representation of the resource.</span></span>

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
