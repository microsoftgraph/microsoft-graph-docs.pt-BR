---
title: tipo de recurso de convertIdResult
description: O resultado de uma conversão de formato de ID realizada pela função translateExchangeIds.
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034470"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="f30ff-103">tipo de recurso de convertIdResult</span><span class="sxs-lookup"><span data-stu-id="f30ff-103">convertIdResult resource type</span></span>

> <span data-ttu-id="f30ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f30ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f30ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f30ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f30ff-106">O resultado de uma conversão de formato de ID realizada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="f30ff-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="f30ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f30ff-107">Properties</span></span>

| <span data-ttu-id="f30ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f30ff-108">Property</span></span> | <span data-ttu-id="f30ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f30ff-109">Type</span></span> | <span data-ttu-id="f30ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f30ff-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f30ff-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="f30ff-111">sourceId</span></span> | <span data-ttu-id="f30ff-112">String</span><span class="sxs-lookup"><span data-stu-id="f30ff-112">String</span></span> | <span data-ttu-id="f30ff-113">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="f30ff-113">The identifier that was converted.</span></span> <span data-ttu-id="f30ff-114">Esse valor é o identificador original, não convertido.</span><span class="sxs-lookup"><span data-stu-id="f30ff-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="f30ff-115">Alvo</span><span class="sxs-lookup"><span data-stu-id="f30ff-115">targetId</span></span> | <span data-ttu-id="f30ff-116">String</span><span class="sxs-lookup"><span data-stu-id="f30ff-116">String</span></span> | <span data-ttu-id="f30ff-117">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="f30ff-117">The converted identifier.</span></span> <span data-ttu-id="f30ff-118">Este valor não estiver presente, se a conversão falhou.</span><span class="sxs-lookup"><span data-stu-id="f30ff-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="f30ff-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="f30ff-119">errorDetails</span></span> | [<span data-ttu-id="f30ff-120">Erro genérico</span><span class="sxs-lookup"><span data-stu-id="f30ff-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="f30ff-121">Um objeto de erro que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="f30ff-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="f30ff-122">Este valor não estiver presente, se a conversão foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f30ff-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f30ff-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f30ff-123">JSON representation</span></span>

<span data-ttu-id="f30ff-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f30ff-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```