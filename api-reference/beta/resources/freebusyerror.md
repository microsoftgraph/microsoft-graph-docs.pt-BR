---
title: tipo de recurso de freeBusyError
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: d1bf6671d6c506d9959fcd5abc8843c1a08c924b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039204"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="fcacf-104">tipo de recurso de freeBusyError</span><span class="sxs-lookup"><span data-stu-id="fcacf-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="fcacf-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fcacf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcacf-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fcacf-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="fcacf-107">Representa informações de erro de tentar obter a disponibilidade de um usuário, uma lista de distribuição ou um recurso.</span><span class="sxs-lookup"><span data-stu-id="fcacf-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="fcacf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcacf-108">Properties</span></span>
| <span data-ttu-id="fcacf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcacf-109">Property</span></span>     | <span data-ttu-id="fcacf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcacf-110">Type</span></span>   |<span data-ttu-id="fcacf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcacf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcacf-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="fcacf-112">message</span></span> |<span data-ttu-id="fcacf-113">String</span><span class="sxs-lookup"><span data-stu-id="fcacf-113">String</span></span> |<span data-ttu-id="fcacf-114">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="fcacf-114">Describes the error.</span></span> |
|<span data-ttu-id="fcacf-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="fcacf-115">responseCode</span></span> |<span data-ttu-id="fcacf-116">String</span><span class="sxs-lookup"><span data-stu-id="fcacf-116">String</span></span> |<span data-ttu-id="fcacf-117">O código de resposta do consultando para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="fcacf-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fcacf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcacf-118">JSON representation</span></span>

<span data-ttu-id="fcacf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fcacf-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->