---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
ms.openlocfilehash: 44769bab4a4f4b40a80d896bed2311554ea5e8ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889856"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="08689-103">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="08689-103">extensionSchemaProperty resource type</span></span>

> <span data-ttu-id="08689-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="08689-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08689-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="08689-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08689-106">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="08689-106">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="08689-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08689-107">Properties</span></span>
| <span data-ttu-id="08689-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08689-108">Property</span></span>     | <span data-ttu-id="08689-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="08689-109">Type</span></span>   |<span data-ttu-id="08689-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08689-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08689-111">name</span><span class="sxs-lookup"><span data-stu-id="08689-111">name</span></span>|<span data-ttu-id="08689-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08689-112">String</span></span>| <span data-ttu-id="08689-113">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="08689-113">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="08689-114">type</span><span class="sxs-lookup"><span data-stu-id="08689-114">type</span></span>|<span data-ttu-id="08689-115">String</span><span class="sxs-lookup"><span data-stu-id="08689-115">String</span></span>| <span data-ttu-id="08689-p102">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="08689-p102">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="08689-119">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="08689-119">Supported property data types</span></span> 
<span data-ttu-id="08689-120">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="08689-120">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="08689-121">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="08689-121">Property Type</span></span> | <span data-ttu-id="08689-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="08689-122">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="08689-123">Binária</span><span class="sxs-lookup"><span data-stu-id="08689-123">Binary</span></span> | <span data-ttu-id="08689-124">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="08689-124">256 bytes maximum.</span></span> |
| <span data-ttu-id="08689-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="08689-125">Boolean</span></span> | <span data-ttu-id="08689-126">Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="08689-126">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="08689-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="08689-127">DateTime</span></span> | <span data-ttu-id="08689-p103">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="08689-p103">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="08689-130">Inteiro</span><span class="sxs-lookup"><span data-stu-id="08689-130">Integer</span></span> | <span data-ttu-id="08689-p104">Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="08689-p104">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="08689-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08689-133">String</span></span> | <span data-ttu-id="08689-134">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="08689-134">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08689-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08689-135">JSON representation</span></span>
<span data-ttu-id="08689-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08689-136">Here is a JSON representation of the resource.</span></span>

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
