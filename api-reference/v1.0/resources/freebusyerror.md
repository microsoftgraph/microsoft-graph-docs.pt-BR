---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8e069aef1d26a409e9ebe29a516136a952604ee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531381"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="24e83-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="24e83-103">freeBusyError resource type</span></span>

<span data-ttu-id="24e83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24e83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24e83-105">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="24e83-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="24e83-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24e83-106">Properties</span></span>
| <span data-ttu-id="24e83-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24e83-107">Property</span></span>     | <span data-ttu-id="24e83-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="24e83-108">Type</span></span>   |<span data-ttu-id="24e83-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e83-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24e83-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="24e83-110">message</span></span> |<span data-ttu-id="24e83-111">String</span><span class="sxs-lookup"><span data-stu-id="24e83-111">String</span></span> |<span data-ttu-id="24e83-112">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="24e83-112">Describes the error.</span></span> |
|<span data-ttu-id="24e83-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="24e83-113">responseCode</span></span> |<span data-ttu-id="24e83-114">String</span><span class="sxs-lookup"><span data-stu-id="24e83-114">String</span></span> |<span data-ttu-id="24e83-115">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="24e83-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="24e83-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24e83-116">JSON representation</span></span>

<span data-ttu-id="24e83-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24e83-117">The following is a JSON representation of the resource.</span></span>

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
