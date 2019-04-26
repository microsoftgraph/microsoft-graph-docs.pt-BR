---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
ms.openlocfilehash: e2c755b51e72adf3ff4efa4de5c9438e70d701e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547492"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="327dc-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="327dc-103">freeBusyError resource type</span></span>

<span data-ttu-id="327dc-104">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="327dc-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="327dc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="327dc-105">Properties</span></span>
| <span data-ttu-id="327dc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="327dc-106">Property</span></span>     | <span data-ttu-id="327dc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="327dc-107">Type</span></span>   |<span data-ttu-id="327dc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="327dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327dc-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="327dc-109">message</span></span> |<span data-ttu-id="327dc-110">String</span><span class="sxs-lookup"><span data-stu-id="327dc-110">String</span></span> |<span data-ttu-id="327dc-111">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="327dc-111">Describes the error.</span></span> |
|<span data-ttu-id="327dc-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="327dc-112">responseCode</span></span> |<span data-ttu-id="327dc-113">String</span><span class="sxs-lookup"><span data-stu-id="327dc-113">String</span></span> |<span data-ttu-id="327dc-114">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="327dc-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="327dc-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="327dc-115">JSON representation</span></span>

<span data-ttu-id="327dc-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="327dc-116">The following is a JSON representation of the resource.</span></span>

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
