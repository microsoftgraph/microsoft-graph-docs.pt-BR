---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 07c708ac2d46e23cc4bdcea233587c910d30fc3e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657711"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="38ac0-105">tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="38ac0-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="38ac0-106">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="38ac0-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="38ac0-107">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="38ac0-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="38ac0-108">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="38ac0-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="38ac0-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="38ac0-109">Methods</span></span>

| <span data-ttu-id="38ac0-110">Método</span><span class="sxs-lookup"><span data-stu-id="38ac0-110">Method</span></span>           | <span data-ttu-id="38ac0-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38ac0-111">Return Type</span></span>    |<span data-ttu-id="38ac0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ac0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38ac0-113">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="38ac0-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="38ac0-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="38ac0-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="38ac0-115">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="38ac0-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38ac0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38ac0-116">Properties</span></span>

> <span data-ttu-id="38ac0-117">**Observação:** Todas as propriedades deste recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38ac0-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="38ac0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38ac0-118">Property</span></span>     | <span data-ttu-id="38ac0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="38ac0-119">Type</span></span>   |<span data-ttu-id="38ac0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ac0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38ac0-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="38ac0-121">completedDateTime</span></span>|<span data-ttu-id="38ac0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ac0-122">DateTimeOffset</span></span>|<span data-ttu-id="38ac0-123">Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="38ac0-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="38ac0-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="38ac0-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="38ac0-125">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="38ac0-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="38ac0-126">id</span><span class="sxs-lookup"><span data-stu-id="38ac0-126">id</span></span>|<span data-ttu-id="38ac0-127">String</span><span class="sxs-lookup"><span data-stu-id="38ac0-127">String</span></span>| <span data-ttu-id="38ac0-128">Chave exclusiva para esta operação.</span><span class="sxs-lookup"><span data-stu-id="38ac0-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="38ac0-129">status</span><span class="sxs-lookup"><span data-stu-id="38ac0-129">status</span></span>|<span data-ttu-id="38ac0-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ac0-130">string</span></span>| <span data-ttu-id="38ac0-131">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="38ac0-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="38ac0-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="38ac0-132">storageLocation</span></span>|<span data-ttu-id="38ac0-133">String</span><span class="sxs-lookup"><span data-stu-id="38ac0-133">String</span></span>|<span data-ttu-id="38ac0-134">O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="38ac0-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="38ac0-135">userId</span><span class="sxs-lookup"><span data-stu-id="38ac0-135">userId</span></span>|<span data-ttu-id="38ac0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38ac0-136">String</span></span>|<span data-ttu-id="38ac0-137">A ID do usuário em que a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="38ac0-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="38ac0-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="38ac0-138">submittedDateTime</span></span>|<span data-ttu-id="38ac0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ac0-139">DateTimeOffset</span></span>|<span data-ttu-id="38ac0-140">Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="38ac0-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="38ac0-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38ac0-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38ac0-142">progresso</span><span class="sxs-lookup"><span data-stu-id="38ac0-142">progress</span></span>|<span data-ttu-id="38ac0-143">Duplo</span><span class="sxs-lookup"><span data-stu-id="38ac0-143">Double</span></span>|<span data-ttu-id="38ac0-144">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="38ac0-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38ac0-145">Relações</span><span class="sxs-lookup"><span data-stu-id="38ac0-145">Relationships</span></span>
<span data-ttu-id="38ac0-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38ac0-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="38ac0-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38ac0-147">JSON representation</span></span>

<span data-ttu-id="38ac0-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38ac0-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
