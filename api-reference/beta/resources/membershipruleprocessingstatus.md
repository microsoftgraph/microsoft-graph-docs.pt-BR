---
title: Tipo de recurso membershipRuleProcessingStatus
description: Representa o status atual do processamento de grupo dinâmico.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864cbd9ea446655c2a0d5f950b28fa6421d2241c
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784882"
---
# <a name="membershipruleprocessingstatus-resource-type"></a><span data-ttu-id="353cc-103">Tipo de recurso membershipRuleProcessingStatus</span><span class="sxs-lookup"><span data-stu-id="353cc-103">membershipRuleProcessingStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="353cc-104">Representa o status atual do processamento de grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="353cc-104">Represents the current status of dynamic group processing.</span></span>

## <a name="properties"></a><span data-ttu-id="353cc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="353cc-105">Properties</span></span>

| <span data-ttu-id="353cc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="353cc-106">Property</span></span> | <span data-ttu-id="353cc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="353cc-107">Type</span></span> | <span data-ttu-id="353cc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="353cc-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="353cc-109">status</span><span class="sxs-lookup"><span data-stu-id="353cc-109">status</span></span> | [<span data-ttu-id="353cc-110">membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="353cc-110">membershipRuleProcessingStatusDetails</span></span>](#membershipruleprocessingstatusdetails-values) | <span data-ttu-id="353cc-111">Status atual de um processamento de grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="353cc-111">Current status of a dynamic group processing.</span></span> <span data-ttu-id="353cc-112">Os valores possíveis `NotStarted` são: `Running` , , e `Succeeded` `Failed` `UnknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="353cc-112">Possible values are: `NotStarted`, `Running`, `Succeeded`, `Failed`, and `UnknownFutureValue`.</span></span>  <br><br> <span data-ttu-id="353cc-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="353cc-113">Required.</span></span> <span data-ttu-id="353cc-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="353cc-114">Read-only.</span></span>|
| <span data-ttu-id="353cc-115">lastMembershipUpdated</span><span class="sxs-lookup"><span data-stu-id="353cc-115">lastMembershipUpdated</span></span> | <span data-ttu-id="353cc-116">edm. DateTime</span><span class="sxs-lookup"><span data-stu-id="353cc-116">edm.DateTime</span></span> | <span data-ttu-id="353cc-117">Data e hora mais recentes quando a associação de um grupo dinâmico foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="353cc-117">Most recent date and time when membership of a dynamic group was updated.</span></span> <br><br> <span data-ttu-id="353cc-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="353cc-118">Optional.</span></span> <span data-ttu-id="353cc-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="353cc-119">Read-only.</span></span>|
| <span data-ttu-id="353cc-120">errorMessage</span><span class="sxs-lookup"><span data-stu-id="353cc-120">errorMessage</span></span> | <span data-ttu-id="353cc-121">String</span><span class="sxs-lookup"><span data-stu-id="353cc-121">String</span></span> | <span data-ttu-id="353cc-122">Mensagem de erro detalhada se o processamento de grupo dinâmico encontrou um erro.</span><span class="sxs-lookup"><span data-stu-id="353cc-122">Detailed error message if dynamic group processing ran into an error.</span></span> <br><br> <span data-ttu-id="353cc-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="353cc-123">Optional.</span></span> <span data-ttu-id="353cc-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="353cc-124">Read-only.</span></span>|

### <a name="membershipruleprocessingstatusdetails-values"></a><span data-ttu-id="353cc-125">Valores de membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="353cc-125">membershipRuleProcessingStatusDetails values</span></span>

| <span data-ttu-id="353cc-126">Member</span><span class="sxs-lookup"><span data-stu-id="353cc-126">Member</span></span> | <span data-ttu-id="353cc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="353cc-127">Description</span></span> |
|:-------- |:----------- |
| <span data-ttu-id="353cc-128">NotStarted</span><span class="sxs-lookup"><span data-stu-id="353cc-128">NotStarted</span></span> | <span data-ttu-id="353cc-129">O grupo foi criado ou atualizado e aguardando processamento.</span><span class="sxs-lookup"><span data-stu-id="353cc-129">Group has been created or updated, and awaiting processing.</span></span>|
| <span data-ttu-id="353cc-130">Em execução</span><span class="sxs-lookup"><span data-stu-id="353cc-130">Running</span></span> | <span data-ttu-id="353cc-131">O processamento foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="353cc-131">Processing has started.</span></span>|
| <span data-ttu-id="353cc-132">Succeeded</span><span class="sxs-lookup"><span data-stu-id="353cc-132">Succeeded</span></span> | <span data-ttu-id="353cc-133">O processamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="353cc-133">Processing has completed.</span></span> <span data-ttu-id="353cc-134">As alterações incrementais de objeto são processadas permanentemente.</span><span class="sxs-lookup"><span data-stu-id="353cc-134">Incremental object changes are processed perpetually.</span></span> |
| <span data-ttu-id="353cc-135">Falhou</span><span class="sxs-lookup"><span data-stu-id="353cc-135">Failed</span></span> | <span data-ttu-id="353cc-136">O processamento encontrou um erro.</span><span class="sxs-lookup"><span data-stu-id="353cc-136">Processing ran into an error.</span></span> <span data-ttu-id="353cc-137">Consulte **errorMessage** para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="353cc-137">See **errorMessage** for details.</span></span> |
| <span data-ttu-id="353cc-138">UnknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="353cc-138">UnknownFutureValue</span></span> | <span data-ttu-id="353cc-139">Oferece suporte a valores futuros.</span><span class="sxs-lookup"><span data-stu-id="353cc-139">Supports future values.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="353cc-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="353cc-140">JSON representation</span></span>

<span data-ttu-id="353cc-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="353cc-141">The following is a JSON representation of the resource.</span></span>

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
