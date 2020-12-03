---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3633968869c0cf61e16afa4ba056a530c86b3c93
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563650"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="6f0a1-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="6f0a1-103">signInStatus resource type</span></span>

<span data-ttu-id="6f0a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f0a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f0a1-105">Fornece o status de entrada (sucesso ou falha) da entrada.</span><span class="sxs-lookup"><span data-stu-id="6f0a1-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="6f0a1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f0a1-106">Properties</span></span>

| <span data-ttu-id="6f0a1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f0a1-107">Property</span></span>     | <span data-ttu-id="6f0a1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f0a1-108">Type</span></span>   |<span data-ttu-id="6f0a1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f0a1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f0a1-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="6f0a1-110">additionalDetails</span></span>|<span data-ttu-id="6f0a1-111">String</span><span class="sxs-lookup"><span data-stu-id="6f0a1-111">String</span></span>|<span data-ttu-id="6f0a1-112">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="6f0a1-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="6f0a1-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="6f0a1-113">errorCode</span></span>|<span data-ttu-id="6f0a1-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0a1-114">Int32</span></span>|<span data-ttu-id="6f0a1-115">Fornece o código de erro de dígito 5-6 gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="6f0a1-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="6f0a1-116">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="6f0a1-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="6f0a1-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="6f0a1-117">failureReason</span></span>|<span data-ttu-id="6f0a1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f0a1-118">String</span></span>|<span data-ttu-id="6f0a1-119">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="6f0a1-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="6f0a1-120">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="6f0a1-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f0a1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f0a1-121">JSON representation</span></span>

<span data-ttu-id="6f0a1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f0a1-122">Here is a JSON representation of the resource.</span></span>

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

