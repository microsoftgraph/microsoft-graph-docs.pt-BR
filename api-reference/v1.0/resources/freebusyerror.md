---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030279"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="d28df-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="d28df-103">freeBusyError resource type</span></span>

<span data-ttu-id="d28df-104">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="d28df-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d28df-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d28df-105">Properties</span></span>
| <span data-ttu-id="d28df-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d28df-106">Property</span></span>     | <span data-ttu-id="d28df-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d28df-107">Type</span></span>   |<span data-ttu-id="d28df-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d28df-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d28df-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="d28df-109">message</span></span> |<span data-ttu-id="d28df-110">String</span><span class="sxs-lookup"><span data-stu-id="d28df-110">String</span></span> |<span data-ttu-id="d28df-111">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="d28df-111">Describes the error.</span></span> |
|<span data-ttu-id="d28df-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="d28df-112">responseCode</span></span> |<span data-ttu-id="d28df-113">String</span><span class="sxs-lookup"><span data-stu-id="d28df-113">String</span></span> |<span data-ttu-id="d28df-114">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="d28df-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d28df-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d28df-115">JSON representation</span></span>

<span data-ttu-id="d28df-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d28df-116">The following is a JSON representation of the resource.</span></span>

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
