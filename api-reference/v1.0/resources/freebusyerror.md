---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b161d47ff7a89c79a04e9400ff0d4756692f49c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018214"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="858c9-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="858c9-103">freeBusyError resource type</span></span>

<span data-ttu-id="858c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="858c9-105">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="858c9-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="858c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="858c9-106">Properties</span></span>
| <span data-ttu-id="858c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="858c9-107">Property</span></span>     | <span data-ttu-id="858c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="858c9-108">Type</span></span>   |<span data-ttu-id="858c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="858c9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="858c9-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="858c9-110">message</span></span> |<span data-ttu-id="858c9-111">String</span><span class="sxs-lookup"><span data-stu-id="858c9-111">String</span></span> |<span data-ttu-id="858c9-112">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="858c9-112">Describes the error.</span></span> |
|<span data-ttu-id="858c9-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="858c9-113">responseCode</span></span> |<span data-ttu-id="858c9-114">String</span><span class="sxs-lookup"><span data-stu-id="858c9-114">String</span></span> |<span data-ttu-id="858c9-115">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="858c9-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="858c9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="858c9-116">JSON representation</span></span>

<span data-ttu-id="858c9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="858c9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

