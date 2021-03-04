---
title: Tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a1d1b1adb9a7de73ecefc6a4290b386d299d784e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440504"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="5d1ee-105">Tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5d1ee-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="5d1ee-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d1ee-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d1ee-107">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="5d1ee-108">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="5d1ee-109">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="5d1ee-110">Methods</span><span class="sxs-lookup"><span data-stu-id="5d1ee-110">Methods</span></span>

| <span data-ttu-id="5d1ee-111">Método</span><span class="sxs-lookup"><span data-stu-id="5d1ee-111">Method</span></span>           | <span data-ttu-id="5d1ee-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d1ee-112">Return Type</span></span>    |<span data-ttu-id="5d1ee-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d1ee-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5d1ee-114">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5d1ee-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="5d1ee-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5d1ee-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="5d1ee-116">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5d1ee-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d1ee-117">Properties</span></span>

> <span data-ttu-id="5d1ee-118">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="5d1ee-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d1ee-119">Property</span></span>     | <span data-ttu-id="5d1ee-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d1ee-120">Type</span></span>   |<span data-ttu-id="5d1ee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d1ee-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d1ee-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d1ee-122">completedDateTime</span></span>|<span data-ttu-id="5d1ee-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d1ee-123">DateTimeOffset</span></span>|<span data-ttu-id="5d1ee-124">Representa quando a solicitação para essa operação de política de dados foi concluída, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5d1ee-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5d1ee-126">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="5d1ee-127">id</span><span class="sxs-lookup"><span data-stu-id="5d1ee-127">id</span></span>|<span data-ttu-id="5d1ee-128">String</span><span class="sxs-lookup"><span data-stu-id="5d1ee-128">String</span></span>| <span data-ttu-id="5d1ee-129">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="5d1ee-130">status</span><span class="sxs-lookup"><span data-stu-id="5d1ee-130">status</span></span>|<span data-ttu-id="5d1ee-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d1ee-131">string</span></span>| <span data-ttu-id="5d1ee-132">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5d1ee-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="5d1ee-133">storageLocation</span></span>|<span data-ttu-id="5d1ee-134">String</span><span class="sxs-lookup"><span data-stu-id="5d1ee-134">String</span></span>|<span data-ttu-id="5d1ee-135">O local da URL para onde os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="5d1ee-136">userId</span><span class="sxs-lookup"><span data-stu-id="5d1ee-136">userId</span></span>|<span data-ttu-id="5d1ee-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d1ee-137">String</span></span>|<span data-ttu-id="5d1ee-138">A id do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="5d1ee-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d1ee-139">submittedDateTime</span></span>|<span data-ttu-id="5d1ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d1ee-140">DateTimeOffset</span></span>|<span data-ttu-id="5d1ee-141">Representa quando a solicitação para essa operação de dados foi enviada, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5d1ee-142">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5d1ee-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5d1ee-143">progresso</span><span class="sxs-lookup"><span data-stu-id="5d1ee-143">progress</span></span>|<span data-ttu-id="5d1ee-144">Duplo</span><span class="sxs-lookup"><span data-stu-id="5d1ee-144">Double</span></span>|<span data-ttu-id="5d1ee-145">Especifica o andamento de uma operação.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d1ee-146">Relações</span><span class="sxs-lookup"><span data-stu-id="5d1ee-146">Relationships</span></span>
<span data-ttu-id="5d1ee-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d1ee-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5d1ee-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d1ee-148">JSON representation</span></span>

<span data-ttu-id="5d1ee-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d1ee-149">Here is a JSON representation of the resource.</span></span>

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


