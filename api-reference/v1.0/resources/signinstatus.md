---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c534ae4c6d881add405e0cd29d39197ce5e79f1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086414"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="57f96-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="57f96-103">signInStatus resource type</span></span>

<span data-ttu-id="57f96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57f96-105">Fornece o status de entrada (sucesso ou falha) da entrada.</span><span class="sxs-lookup"><span data-stu-id="57f96-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="57f96-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57f96-106">Properties</span></span>

| <span data-ttu-id="57f96-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57f96-107">Property</span></span>     | <span data-ttu-id="57f96-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="57f96-108">Type</span></span>   |<span data-ttu-id="57f96-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="57f96-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57f96-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="57f96-110">additionalDetails</span></span>|<span data-ttu-id="57f96-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57f96-111">String</span></span>|<span data-ttu-id="57f96-112">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="57f96-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="57f96-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="57f96-113">errorCode</span></span>|<span data-ttu-id="57f96-114">Int32</span><span class="sxs-lookup"><span data-stu-id="57f96-114">Int32</span></span>|<span data-ttu-id="57f96-115">Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="57f96-115">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="57f96-116">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="57f96-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="57f96-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="57f96-117">failureReason</span></span>|<span data-ttu-id="57f96-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57f96-118">String</span></span>|<span data-ttu-id="57f96-119">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="57f96-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="57f96-120">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="57f96-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57f96-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57f96-121">JSON representation</span></span>

<span data-ttu-id="57f96-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57f96-122">Here is a JSON representation of the resource.</span></span>

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

