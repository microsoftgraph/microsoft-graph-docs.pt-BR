---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 7cb48f7a4235b28231ab93fc3ccfba074f80d286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808596"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="8ac90-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="8ac90-103">signInStatus resource type</span></span>

<span data-ttu-id="8ac90-104">Namespace: o Microsoft. Graph fornece o status de entrada (êxito ou falha) da entrada</span><span class="sxs-lookup"><span data-stu-id="8ac90-104">Namespace: microsoft.graph Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="8ac90-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ac90-105">Properties</span></span>
| <span data-ttu-id="8ac90-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ac90-106">Property</span></span>     | <span data-ttu-id="8ac90-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ac90-107">Type</span></span>   |<span data-ttu-id="8ac90-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ac90-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ac90-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="8ac90-109">additionalDetails</span></span>|<span data-ttu-id="8ac90-110">String</span><span class="sxs-lookup"><span data-stu-id="8ac90-110">String</span></span>|<span data-ttu-id="8ac90-111">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="8ac90-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="8ac90-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="8ac90-112">errorCode</span></span>|<span data-ttu-id="8ac90-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8ac90-113">Int32</span></span>|<span data-ttu-id="8ac90-114">Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="8ac90-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="8ac90-115">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="8ac90-115">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="8ac90-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="8ac90-116">failureReason</span></span>|<span data-ttu-id="8ac90-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ac90-117">String</span></span>|<span data-ttu-id="8ac90-118">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="8ac90-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="8ac90-119">Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="8ac90-119">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ac90-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ac90-120">JSON representation</span></span>

<span data-ttu-id="8ac90-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ac90-121">Here is a JSON representation of the resource.</span></span>

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
