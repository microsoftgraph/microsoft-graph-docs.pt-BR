---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97f564ed8e17eed8a3e4c24b7dc2e012bdb9ec6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034192"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="53546-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="53546-103">signInStatus resource type</span></span>

<span data-ttu-id="53546-104">Fornece o status de entrada (sucesso ou falha) da entrada.</span><span class="sxs-lookup"><span data-stu-id="53546-104">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="53546-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53546-105">Properties</span></span>

| <span data-ttu-id="53546-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53546-106">Property</span></span>     | <span data-ttu-id="53546-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="53546-107">Type</span></span>   |<span data-ttu-id="53546-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="53546-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53546-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="53546-109">additionalDetails</span></span>|<span data-ttu-id="53546-110">String</span><span class="sxs-lookup"><span data-stu-id="53546-110">String</span></span>|<span data-ttu-id="53546-111">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="53546-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="53546-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="53546-112">errorCode</span></span>|<span data-ttu-id="53546-113">Int32</span><span class="sxs-lookup"><span data-stu-id="53546-113">Int32</span></span>|<span data-ttu-id="53546-114">Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="53546-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="53546-115">Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="53546-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="53546-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="53546-116">failureReason</span></span>|<span data-ttu-id="53546-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53546-117">String</span></span>|<span data-ttu-id="53546-118">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="53546-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="53546-119">Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="53546-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53546-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53546-120">JSON representation</span></span>

<span data-ttu-id="53546-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53546-121">Here is a JSON representation of the resource.</span></span>

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
