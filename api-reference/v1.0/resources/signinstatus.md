---
title: Tipo de recurso signInStatus
description: Fornece o status de login (Êxito ou Falha) da assinatura
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 37eb91434fd7a5fb0dc65f5c7203effd42f3878e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137085"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="be497-103">Tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="be497-103">signInStatus resource type</span></span>

<span data-ttu-id="be497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be497-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be497-105">Fornece o status de login (Êxito ou Falha) da login.</span><span class="sxs-lookup"><span data-stu-id="be497-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="be497-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be497-106">Properties</span></span>

| <span data-ttu-id="be497-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be497-107">Property</span></span>     | <span data-ttu-id="be497-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="be497-108">Type</span></span>   |<span data-ttu-id="be497-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="be497-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be497-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="be497-110">additionalDetails</span></span>|<span data-ttu-id="be497-111">String</span><span class="sxs-lookup"><span data-stu-id="be497-111">String</span></span>|<span data-ttu-id="be497-112">Fornece detalhes adicionais sobre a atividade de login</span><span class="sxs-lookup"><span data-stu-id="be497-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="be497-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="be497-113">errorCode</span></span>|<span data-ttu-id="be497-114">Int32</span><span class="sxs-lookup"><span data-stu-id="be497-114">Int32</span></span>|<span data-ttu-id="be497-115">Fornece o código de erro de 5 a 6 dígitos gerado durante uma falha de login.</span><span class="sxs-lookup"><span data-stu-id="be497-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="be497-116">Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="be497-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="be497-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="be497-117">failureReason</span></span>|<span data-ttu-id="be497-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be497-118">String</span></span>|<span data-ttu-id="be497-119">Fornece a mensagem de erro ou o motivo da falha para a atividade de login correspondente.</span><span class="sxs-lookup"><span data-stu-id="be497-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="be497-120">Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="be497-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be497-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be497-121">JSON representation</span></span>

<span data-ttu-id="be497-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be497-122">Here is a JSON representation of the resource.</span></span>

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

