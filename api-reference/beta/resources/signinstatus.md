---
title: tipo de recurso de signInStatus
description: Fornece o status de entrada (sucesso ou falha) do sign-in
ms.openlocfilehash: cafa0dffe1b1d798d87225ac82901cf041d5e4fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039985"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="2dbdf-103">tipo de recurso de signInStatus</span><span class="sxs-lookup"><span data-stu-id="2dbdf-103">signInStatus resource type</span></span>
<span data-ttu-id="2dbdf-104">Fornece o status de entrada (sucesso ou falha) do sign-in</span><span class="sxs-lookup"><span data-stu-id="2dbdf-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="2dbdf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dbdf-105">Properties</span></span>
| <span data-ttu-id="2dbdf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dbdf-106">Property</span></span>     | <span data-ttu-id="2dbdf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dbdf-107">Type</span></span>   |<span data-ttu-id="2dbdf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dbdf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dbdf-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="2dbdf-109">additionalDetails</span></span>|<span data-ttu-id="2dbdf-110">String</span><span class="sxs-lookup"><span data-stu-id="2dbdf-110">String</span></span>|<span data-ttu-id="2dbdf-111">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="2dbdf-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="2dbdf-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="2dbdf-112">errorCode</span></span>|<span data-ttu-id="2dbdf-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2dbdf-113">Int32</span></span>|<span data-ttu-id="2dbdf-114">Fornece o código de erro 5-6digit gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="2dbdf-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="2dbdf-115">Confira a [lista de mensagens e códigos de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2dbdf-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="2dbdf-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="2dbdf-116">failureReason</span></span>|<span data-ttu-id="2dbdf-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dbdf-117">String</span></span>|<span data-ttu-id="2dbdf-118">Fornece a mensagem de erro ou o motivo da falha da atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="2dbdf-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="2dbdf-119">Confira a [lista de mensagens e códigos de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2dbdf-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dbdf-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dbdf-120">JSON representation</span></span>

<span data-ttu-id="2dbdf-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dbdf-121">Here is a JSON representation of the resource.</span></span>

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