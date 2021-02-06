---
title: Tipo de recurso requestSchedule
description: Um agendamento de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 74fa9589552ba860962c73814e66332eda1c8e8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132535"
---
# <a name="requestschedule-resource-type"></a><span data-ttu-id="74707-103">Tipo de recurso requestSchedule</span><span class="sxs-lookup"><span data-stu-id="74707-103">requestSchedule resource type</span></span>

<span data-ttu-id="74707-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74707-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74707-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="74707-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="74707-106">Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="74707-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="74707-107">Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.</span><span class="sxs-lookup"><span data-stu-id="74707-107">An access package assignment that results from such a request also has a schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="74707-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74707-108">Properties</span></span>

| <span data-ttu-id="74707-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74707-109">Property</span></span>     | <span data-ttu-id="74707-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="74707-110">Type</span></span>        | <span data-ttu-id="74707-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74707-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74707-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="74707-112">startDateTime</span></span>|<span data-ttu-id="74707-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74707-113">DateTimeOffset</span></span>|<span data-ttu-id="74707-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="74707-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74707-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="74707-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="74707-116">expiration</span><span class="sxs-lookup"><span data-stu-id="74707-116">expiration</span></span>|[<span data-ttu-id="74707-117">expirationPattern</span><span class="sxs-lookup"><span data-stu-id="74707-117">expirationPattern</span></span>](expirationpattern.md)|<span data-ttu-id="74707-118">Quando o acesso deve expirar.</span><span class="sxs-lookup"><span data-stu-id="74707-118">When the access should expire.</span></span>|
|<span data-ttu-id="74707-119">recurrence</span><span class="sxs-lookup"><span data-stu-id="74707-119">recurrence</span></span>|[<span data-ttu-id="74707-120">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="74707-120">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="74707-121">Para acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="74707-121">For recurring access.</span></span> <span data-ttu-id="74707-122">Não usado no momento.</span><span class="sxs-lookup"><span data-stu-id="74707-122">Not used at present.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74707-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74707-123">JSON representation</span></span>

<span data-ttu-id="74707-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74707-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


