---
title: Tipo de recurso signInStatus
description: Fornece o status de login (Êxito ou Falha) da login
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d7428c2a73d0b4a114599dad8ac1740d91ba5865
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132633"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="3323d-103">Tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="3323d-103">signInStatus resource type</span></span>

<span data-ttu-id="3323d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3323d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3323d-105">Fornece o status de login (Êxito ou Falha) da login</span><span class="sxs-lookup"><span data-stu-id="3323d-105">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="3323d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3323d-106">Properties</span></span>
| <span data-ttu-id="3323d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3323d-107">Property</span></span>     | <span data-ttu-id="3323d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3323d-108">Type</span></span>   |<span data-ttu-id="3323d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3323d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3323d-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="3323d-110">additionalDetails</span></span>|<span data-ttu-id="3323d-111">String</span><span class="sxs-lookup"><span data-stu-id="3323d-111">String</span></span>|<span data-ttu-id="3323d-112">Fornece detalhes adicionais sobre a atividade de login</span><span class="sxs-lookup"><span data-stu-id="3323d-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="3323d-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="3323d-113">errorCode</span></span>|<span data-ttu-id="3323d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3323d-114">Int32</span></span>|<span data-ttu-id="3323d-115">Fornece o código de erro de 5 a 6 dígitos gerado durante uma falha de login.</span><span class="sxs-lookup"><span data-stu-id="3323d-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="3323d-116">Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="3323d-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="3323d-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="3323d-117">failureReason</span></span>|<span data-ttu-id="3323d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3323d-118">String</span></span>|<span data-ttu-id="3323d-119">Fornece a mensagem de erro ou o motivo da falha para a atividade de login correspondente.</span><span class="sxs-lookup"><span data-stu-id="3323d-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="3323d-120">Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="3323d-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3323d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3323d-121">JSON representation</span></span>

<span data-ttu-id="3323d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3323d-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


