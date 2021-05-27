---
title: Tipo de recurso membershipRuleProcessingStatus
description: Representa o status atual do processamento dinâmico do grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c86f044517ad7b808db69364413727c8d76f076
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680994"
---
# <a name="membershipruleprocessingstatus-resource-type"></a><span data-ttu-id="6afae-103">Tipo de recurso membershipRuleProcessingStatus</span><span class="sxs-lookup"><span data-stu-id="6afae-103">membershipRuleProcessingStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6afae-104">Representa o status atual do processamento dinâmico do grupo.</span><span class="sxs-lookup"><span data-stu-id="6afae-104">Represents the current status of dynamic group processing.</span></span>

## <a name="properties"></a><span data-ttu-id="6afae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6afae-105">Properties</span></span>

| <span data-ttu-id="6afae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6afae-106">Property</span></span> | <span data-ttu-id="6afae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6afae-107">Type</span></span> | <span data-ttu-id="6afae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6afae-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6afae-109">status</span><span class="sxs-lookup"><span data-stu-id="6afae-109">status</span></span> | [<span data-ttu-id="6afae-110">membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="6afae-110">membershipRuleProcessingStatusDetails</span></span>](#membershipruleprocessingstatusdetails-values) | <span data-ttu-id="6afae-111">Status atual de um processamento dinâmico de grupo.</span><span class="sxs-lookup"><span data-stu-id="6afae-111">Current status of a dynamic group processing.</span></span> <span data-ttu-id="6afae-112">Os valores possíveis são: `NotStarted` , , , e `Running` `Succeeded` `Failed` `UnknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="6afae-112">Possible values are: `NotStarted`, `Running`, `Succeeded`, `Failed`, and `UnknownFutureValue`.</span></span>  <br><br> <span data-ttu-id="6afae-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6afae-113">Required.</span></span> <span data-ttu-id="6afae-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6afae-114">Read-only.</span></span>|
| <span data-ttu-id="6afae-115">lastMembershipUpdated</span><span class="sxs-lookup"><span data-stu-id="6afae-115">lastMembershipUpdated</span></span> | <span data-ttu-id="6afae-116">edm. DateTime</span><span class="sxs-lookup"><span data-stu-id="6afae-116">edm.DateTime</span></span> | <span data-ttu-id="6afae-117">Data e hora mais recentes em que a associação de um grupo dinâmico foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="6afae-117">Most recent date and time when membership of a dynamic group was updated.</span></span> <br><br> <span data-ttu-id="6afae-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6afae-118">Optional.</span></span> <span data-ttu-id="6afae-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6afae-119">Read-only.</span></span>|
| <span data-ttu-id="6afae-120">errorMessage</span><span class="sxs-lookup"><span data-stu-id="6afae-120">errorMessage</span></span> | <span data-ttu-id="6afae-121">String</span><span class="sxs-lookup"><span data-stu-id="6afae-121">String</span></span> | <span data-ttu-id="6afae-122">Mensagem de erro detalhada se o processamento dinâmico de grupo ocorreu em um erro.</span><span class="sxs-lookup"><span data-stu-id="6afae-122">Detailed error message if dynamic group processing ran into an error.</span></span> <br><br> <span data-ttu-id="6afae-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6afae-123">Optional.</span></span> <span data-ttu-id="6afae-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6afae-124">Read-only.</span></span>|

### <a name="membershipruleprocessingstatusdetails-values"></a><span data-ttu-id="6afae-125">membershipRuleProcessingStatusDetails values</span><span class="sxs-lookup"><span data-stu-id="6afae-125">membershipRuleProcessingStatusDetails values</span></span>

| <span data-ttu-id="6afae-126">Member</span><span class="sxs-lookup"><span data-stu-id="6afae-126">Member</span></span> | <span data-ttu-id="6afae-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6afae-127">Description</span></span> |
|:-------- |:----------- |
| <span data-ttu-id="6afae-128">NotStarted</span><span class="sxs-lookup"><span data-stu-id="6afae-128">NotStarted</span></span> | <span data-ttu-id="6afae-129">O grupo foi criado ou atualizado e aguarda processamento.</span><span class="sxs-lookup"><span data-stu-id="6afae-129">Group has been created or updated, and awaiting processing.</span></span>|
| <span data-ttu-id="6afae-130">Em execução</span><span class="sxs-lookup"><span data-stu-id="6afae-130">Running</span></span> | <span data-ttu-id="6afae-131">O processamento foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="6afae-131">Processing has started.</span></span>|
| <span data-ttu-id="6afae-132">Succeeded</span><span class="sxs-lookup"><span data-stu-id="6afae-132">Succeeded</span></span> | <span data-ttu-id="6afae-133">O processamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="6afae-133">Processing has completed.</span></span> <span data-ttu-id="6afae-134">As alterações incrementais do objeto são processadas permanentemente.</span><span class="sxs-lookup"><span data-stu-id="6afae-134">Incremental object changes are processed perpetually.</span></span> |
| <span data-ttu-id="6afae-135">Falhou</span><span class="sxs-lookup"><span data-stu-id="6afae-135">Failed</span></span> | <span data-ttu-id="6afae-136">O processamento ocorreu em um erro.</span><span class="sxs-lookup"><span data-stu-id="6afae-136">Processing ran into an error.</span></span> <span data-ttu-id="6afae-137">Consulte **errorMessage** para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="6afae-137">See **errorMessage** for details.</span></span> |
| <span data-ttu-id="6afae-138">UnknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="6afae-138">UnknownFutureValue</span></span> | <span data-ttu-id="6afae-139">Oferece suporte a valores futuros.</span><span class="sxs-lookup"><span data-stu-id="6afae-139">Supports future values.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6afae-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6afae-140">JSON representation</span></span>

<span data-ttu-id="6afae-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6afae-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```
