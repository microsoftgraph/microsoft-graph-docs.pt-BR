---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c6f78a666d5e3785c6e02b9f5622f5d0529c61a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507307"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="da52d-105">tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="da52d-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="da52d-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da52d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da52d-107">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="da52d-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="da52d-108">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="da52d-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="da52d-109">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="da52d-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="da52d-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="da52d-110">Methods</span></span>

| <span data-ttu-id="da52d-111">Método</span><span class="sxs-lookup"><span data-stu-id="da52d-111">Method</span></span>           | <span data-ttu-id="da52d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="da52d-112">Return Type</span></span>    |<span data-ttu-id="da52d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="da52d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da52d-114">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="da52d-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="da52d-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="da52d-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="da52d-116">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="da52d-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da52d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da52d-117">Properties</span></span>

> <span data-ttu-id="da52d-118">**Observação:** Todas as propriedades deste recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da52d-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="da52d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da52d-119">Property</span></span>     | <span data-ttu-id="da52d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="da52d-120">Type</span></span>   |<span data-ttu-id="da52d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="da52d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da52d-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="da52d-122">completedDateTime</span></span>|<span data-ttu-id="da52d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da52d-123">DateTimeOffset</span></span>|<span data-ttu-id="da52d-124">Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="da52d-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="da52d-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="da52d-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="da52d-126">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="da52d-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="da52d-127">id</span><span class="sxs-lookup"><span data-stu-id="da52d-127">id</span></span>|<span data-ttu-id="da52d-128">String</span><span class="sxs-lookup"><span data-stu-id="da52d-128">String</span></span>| <span data-ttu-id="da52d-129">Chave exclusiva para esta operação.</span><span class="sxs-lookup"><span data-stu-id="da52d-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="da52d-130">status</span><span class="sxs-lookup"><span data-stu-id="da52d-130">status</span></span>|<span data-ttu-id="da52d-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da52d-131">string</span></span>| <span data-ttu-id="da52d-132">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da52d-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="da52d-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="da52d-133">storageLocation</span></span>|<span data-ttu-id="da52d-134">String</span><span class="sxs-lookup"><span data-stu-id="da52d-134">String</span></span>|<span data-ttu-id="da52d-135">O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="da52d-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="da52d-136">userId</span><span class="sxs-lookup"><span data-stu-id="da52d-136">userId</span></span>|<span data-ttu-id="da52d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da52d-137">String</span></span>|<span data-ttu-id="da52d-138">A ID do usuário em que a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="da52d-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="da52d-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="da52d-139">submittedDateTime</span></span>|<span data-ttu-id="da52d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da52d-140">DateTimeOffset</span></span>|<span data-ttu-id="da52d-141">Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="da52d-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="da52d-142">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="da52d-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="da52d-143">progresso</span><span class="sxs-lookup"><span data-stu-id="da52d-143">progress</span></span>|<span data-ttu-id="da52d-144">Duplo</span><span class="sxs-lookup"><span data-stu-id="da52d-144">Double</span></span>|<span data-ttu-id="da52d-145">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="da52d-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da52d-146">Relações</span><span class="sxs-lookup"><span data-stu-id="da52d-146">Relationships</span></span>
<span data-ttu-id="da52d-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da52d-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="da52d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da52d-148">JSON representation</span></span>

<span data-ttu-id="da52d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da52d-149">Here is a JSON representation of the resource.</span></span>

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
