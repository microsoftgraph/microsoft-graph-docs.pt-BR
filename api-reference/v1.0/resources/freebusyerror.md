---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 019c21eadc65b29d74bdc6fd94c40641acd43491
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812257"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="8714e-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="8714e-103">freeBusyError resource type</span></span>

<span data-ttu-id="8714e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8714e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8714e-105">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="8714e-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="8714e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8714e-106">Properties</span></span>
| <span data-ttu-id="8714e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8714e-107">Property</span></span>     | <span data-ttu-id="8714e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8714e-108">Type</span></span>   |<span data-ttu-id="8714e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8714e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8714e-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="8714e-110">message</span></span> |<span data-ttu-id="8714e-111">String</span><span class="sxs-lookup"><span data-stu-id="8714e-111">String</span></span> |<span data-ttu-id="8714e-112">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="8714e-112">Describes the error.</span></span> |
|<span data-ttu-id="8714e-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="8714e-113">responseCode</span></span> |<span data-ttu-id="8714e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8714e-114">String</span></span> |<span data-ttu-id="8714e-115">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="8714e-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8714e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8714e-116">JSON representation</span></span>

<span data-ttu-id="8714e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8714e-117">The following is a JSON representation of the resource.</span></span>

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
