---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b88a450465798386ad57e82ff76896417301a606
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817630"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="aa6c6-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="aa6c6-103">outlookItem resource type</span></span>

> <span data-ttu-id="aa6c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa6c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa6c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa6c6-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa6c6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa6c6-106">JSON representation</span></span>

<span data-ttu-id="aa6c6-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="aa6c6-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="aa6c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa6c6-108">Properties</span></span>
| <span data-ttu-id="aa6c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa6c6-109">Property</span></span>     | <span data-ttu-id="aa6c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa6c6-110">Type</span></span>   |<span data-ttu-id="aa6c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa6c6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6c6-112">categories</span><span class="sxs-lookup"><span data-stu-id="aa6c6-112">categories</span></span>|<span data-ttu-id="aa6c6-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa6c6-113">String collection</span></span>||
|<span data-ttu-id="aa6c6-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="aa6c6-114">changeKey</span></span>|<span data-ttu-id="aa6c6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa6c6-115">String</span></span>||
|<span data-ttu-id="aa6c6-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa6c6-116">createdDateTime</span></span>|<span data-ttu-id="aa6c6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa6c6-117">DateTimeOffset</span></span>|<span data-ttu-id="aa6c6-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="aa6c6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="aa6c6-120">id</span><span class="sxs-lookup"><span data-stu-id="aa6c6-120">id</span></span>|<span data-ttu-id="aa6c6-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa6c6-121">String</span></span>| <span data-ttu-id="aa6c6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa6c6-122">Read-only.</span></span>|
|<span data-ttu-id="aa6c6-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa6c6-123">lastModifiedDateTime</span></span>|<span data-ttu-id="aa6c6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa6c6-124">DateTimeOffset</span></span>|<span data-ttu-id="aa6c6-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="aa6c6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa6c6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="aa6c6-127">Relationships</span></span>
<span data-ttu-id="aa6c6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa6c6-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
