---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a57e5bb0e53f5deec4d0c6d92541f7d2bd4744d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629219"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="d74d3-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="d74d3-103">signInStatus resource type</span></span>

<span data-ttu-id="d74d3-104">Fornece o status de entrada (sucesso ou falha) da entrada.</span><span class="sxs-lookup"><span data-stu-id="d74d3-104">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="d74d3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d74d3-105">Properties</span></span>

| <span data-ttu-id="d74d3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d74d3-106">Property</span></span>     | <span data-ttu-id="d74d3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d74d3-107">Type</span></span>   |<span data-ttu-id="d74d3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74d3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d74d3-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="d74d3-109">additionalDetails</span></span>|<span data-ttu-id="d74d3-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d74d3-110">String</span></span>|<span data-ttu-id="d74d3-111">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="d74d3-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="d74d3-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="d74d3-112">errorCode</span></span>|<span data-ttu-id="d74d3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d74d3-113">Int32</span></span>|<span data-ttu-id="d74d3-114">Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="d74d3-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="d74d3-115">Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="d74d3-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="d74d3-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="d74d3-116">failureReason</span></span>|<span data-ttu-id="d74d3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d74d3-117">String</span></span>|<span data-ttu-id="d74d3-118">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="d74d3-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="d74d3-119">Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="d74d3-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d74d3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d74d3-120">JSON representation</span></span>

<span data-ttu-id="d74d3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d74d3-121">Here is a JSON representation of the resource.</span></span>

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
