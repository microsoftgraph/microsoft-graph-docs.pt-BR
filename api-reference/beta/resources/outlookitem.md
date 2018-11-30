---
title: Tipo de recurso outlookItem
description: Veja a seguir uma representação JSON do recurso
ms.openlocfilehash: 6de0b5f9f79f8c3f813cbd876fa22f6b43f71a53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039746"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="f7386-103">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="f7386-103">outlookItem resource type</span></span>

> <span data-ttu-id="f7386-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7386-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7386-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7386-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7386-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7386-106">JSON representation</span></span>

<span data-ttu-id="f7386-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f7386-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f7386-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7386-108">Properties</span></span>
| <span data-ttu-id="f7386-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7386-109">Property</span></span>     | <span data-ttu-id="f7386-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7386-110">Type</span></span>   |<span data-ttu-id="f7386-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7386-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7386-112">categories</span><span class="sxs-lookup"><span data-stu-id="f7386-112">categories</span></span>|<span data-ttu-id="f7386-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7386-113">String collection</span></span>||
|<span data-ttu-id="f7386-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="f7386-114">changeKey</span></span>|<span data-ttu-id="f7386-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7386-115">String</span></span>||
|<span data-ttu-id="f7386-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7386-116">createdDateTime</span></span>|<span data-ttu-id="f7386-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7386-117">DateTimeOffset</span></span>|<span data-ttu-id="f7386-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f7386-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f7386-120">id</span><span class="sxs-lookup"><span data-stu-id="f7386-120">id</span></span>|<span data-ttu-id="f7386-121">String</span><span class="sxs-lookup"><span data-stu-id="f7386-121">String</span></span>| <span data-ttu-id="f7386-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7386-122">Read-only.</span></span>|
|<span data-ttu-id="f7386-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7386-123">lastModifiedDateTime</span></span>|<span data-ttu-id="f7386-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7386-124">DateTimeOffset</span></span>|<span data-ttu-id="f7386-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f7386-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7386-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f7386-127">Relationships</span></span>
<span data-ttu-id="f7386-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7386-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->