---
title: tipo de recurso de dataPolicyOperation
description: Representa uma operação de diretiva de dados enviados. Ele contém as informações necessárias para rastrear o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.
ms.openlocfilehash: e6763f4050157658ea0a7f4d1e6f52668ed6e4b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038621"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="fa051-105">tipo de recurso de dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa051-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="fa051-106">Representa uma operação de diretiva de dados enviados.</span><span class="sxs-lookup"><span data-stu-id="fa051-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="fa051-107">Ele contém as informações necessárias para rastrear o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="fa051-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="fa051-108">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa051-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="fa051-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="fa051-109">Methods</span></span>

| <span data-ttu-id="fa051-110">Método</span><span class="sxs-lookup"><span data-stu-id="fa051-110">Method</span></span>           | <span data-ttu-id="fa051-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fa051-111">Return Type</span></span>    |<span data-ttu-id="fa051-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa051-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa051-113">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa051-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="fa051-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa051-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="fa051-115">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="fa051-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa051-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa051-116">Properties</span></span>

> <span data-ttu-id="fa051-117">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa051-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="fa051-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa051-118">Property</span></span>     | <span data-ttu-id="fa051-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa051-119">Type</span></span>   |<span data-ttu-id="fa051-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa051-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa051-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa051-121">completedDateTime</span></span>|<span data-ttu-id="fa051-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa051-122">DateTimeOffset</span></span>|<span data-ttu-id="fa051-123">Representa quando a solicitação para esta operação de política de dados foi concluída, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fa051-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fa051-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa051-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fa051-125">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="fa051-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="fa051-126">id</span><span class="sxs-lookup"><span data-stu-id="fa051-126">id</span></span>|<span data-ttu-id="fa051-127">String</span><span class="sxs-lookup"><span data-stu-id="fa051-127">String</span></span>| <span data-ttu-id="fa051-128">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="fa051-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="fa051-129">status</span><span class="sxs-lookup"><span data-stu-id="fa051-129">status</span></span>|<span data-ttu-id="fa051-130">string</span><span class="sxs-lookup"><span data-stu-id="fa051-130">string</span></span>| <span data-ttu-id="fa051-131">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fa051-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fa051-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="fa051-132">storageLocation</span></span>|<span data-ttu-id="fa051-133">String</span><span class="sxs-lookup"><span data-stu-id="fa051-133">String</span></span>|<span data-ttu-id="fa051-134">O local da URL para onde os dados está sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="fa051-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="fa051-135">userId</span><span class="sxs-lookup"><span data-stu-id="fa051-135">userId</span></span>|<span data-ttu-id="fa051-136">String</span><span class="sxs-lookup"><span data-stu-id="fa051-136">String</span></span>|<span data-ttu-id="fa051-137">A identificação do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="fa051-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="fa051-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa051-138">submittedDateTime</span></span>|<span data-ttu-id="fa051-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa051-139">DateTimeOffset</span></span>|<span data-ttu-id="fa051-140">Representa quando a solicitação para esta operação de dados foi enviada, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fa051-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fa051-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fa051-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa051-142">Relações</span><span class="sxs-lookup"><span data-stu-id="fa051-142">Relationships</span></span>
<span data-ttu-id="fa051-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa051-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fa051-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa051-144">JSON representation</span></span>

<span data-ttu-id="fa051-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa051-145">Here is a JSON representation of the resource.</span></span>

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
  "submittedDateTime": "String (timestamp)"
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
