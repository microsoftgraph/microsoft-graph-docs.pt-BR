---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583568"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="2be07-103">tipo de recurso signInStatus</span><span class="sxs-lookup"><span data-stu-id="2be07-103">signInStatus resource type</span></span>
<span data-ttu-id="2be07-104">Fornece o status de entrada (sucesso ou falha) da entrada</span><span class="sxs-lookup"><span data-stu-id="2be07-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="2be07-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2be07-105">Properties</span></span>
| <span data-ttu-id="2be07-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2be07-106">Property</span></span>     | <span data-ttu-id="2be07-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2be07-107">Type</span></span>   |<span data-ttu-id="2be07-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2be07-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2be07-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="2be07-109">additionalDetails</span></span>|<span data-ttu-id="2be07-110">String</span><span class="sxs-lookup"><span data-stu-id="2be07-110">String</span></span>|<span data-ttu-id="2be07-111">Fornece detalhes adicionais sobre a atividade de entrada</span><span class="sxs-lookup"><span data-stu-id="2be07-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="2be07-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="2be07-112">errorCode</span></span>|<span data-ttu-id="2be07-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2be07-113">Int32</span></span>|<span data-ttu-id="2be07-114">Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada.</span><span class="sxs-lookup"><span data-stu-id="2be07-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="2be07-115">ConFira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2be07-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="2be07-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="2be07-116">failureReason</span></span>|<span data-ttu-id="2be07-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2be07-117">String</span></span>|<span data-ttu-id="2be07-118">Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente.</span><span class="sxs-lookup"><span data-stu-id="2be07-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="2be07-119">ConFira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2be07-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2be07-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2be07-120">JSON representation</span></span>

<span data-ttu-id="2be07-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2be07-121">Here is a JSON representation of the resource.</span></span>

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
