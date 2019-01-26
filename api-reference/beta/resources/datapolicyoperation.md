---
title: tipo de recurso de dataPolicyOperation
description: Representa uma operação de diretiva de dados enviados. Ele contém as informações necessárias para rastrear o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4547221c8c1b859d4738a5468603ac6890246263
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570922"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="d4cdf-105">tipo de recurso de dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4cdf-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="d4cdf-106">Representa uma operação de diretiva de dados enviados.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="d4cdf-107">Ele contém as informações necessárias para rastrear o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="d4cdf-108">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="d4cdf-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4cdf-109">Methods</span></span>

| <span data-ttu-id="d4cdf-110">Método</span><span class="sxs-lookup"><span data-stu-id="d4cdf-110">Method</span></span>           | <span data-ttu-id="d4cdf-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4cdf-111">Return Type</span></span>    |<span data-ttu-id="d4cdf-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4cdf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4cdf-113">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4cdf-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="d4cdf-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4cdf-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="d4cdf-115">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4cdf-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4cdf-116">Properties</span></span>

> <span data-ttu-id="d4cdf-117">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="d4cdf-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4cdf-118">Property</span></span>     | <span data-ttu-id="d4cdf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4cdf-119">Type</span></span>   |<span data-ttu-id="d4cdf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4cdf-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4cdf-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cdf-121">completedDateTime</span></span>|<span data-ttu-id="d4cdf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cdf-122">DateTimeOffset</span></span>|<span data-ttu-id="d4cdf-123">Representa quando a solicitação para esta operação de política de dados foi concluída, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4cdf-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d4cdf-125">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="d4cdf-126">id</span><span class="sxs-lookup"><span data-stu-id="d4cdf-126">id</span></span>|<span data-ttu-id="d4cdf-127">String</span><span class="sxs-lookup"><span data-stu-id="d4cdf-127">String</span></span>| <span data-ttu-id="d4cdf-128">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="d4cdf-129">status</span><span class="sxs-lookup"><span data-stu-id="d4cdf-129">status</span></span>|<span data-ttu-id="d4cdf-130">string</span><span class="sxs-lookup"><span data-stu-id="d4cdf-130">string</span></span>| <span data-ttu-id="d4cdf-131">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4cdf-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="d4cdf-132">storageLocation</span></span>|<span data-ttu-id="d4cdf-133">String</span><span class="sxs-lookup"><span data-stu-id="d4cdf-133">String</span></span>|<span data-ttu-id="d4cdf-134">O local da URL para onde os dados está sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="d4cdf-135">userId</span><span class="sxs-lookup"><span data-stu-id="d4cdf-135">userId</span></span>|<span data-ttu-id="d4cdf-136">String</span><span class="sxs-lookup"><span data-stu-id="d4cdf-136">String</span></span>|<span data-ttu-id="d4cdf-137">A identificação do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="d4cdf-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cdf-138">submittedDateTime</span></span>|<span data-ttu-id="d4cdf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cdf-139">DateTimeOffset</span></span>|<span data-ttu-id="d4cdf-140">Representa quando a solicitação para esta operação de dados foi enviada, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4cdf-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4cdf-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4cdf-142">Relações</span><span class="sxs-lookup"><span data-stu-id="d4cdf-142">Relationships</span></span>
<span data-ttu-id="d4cdf-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4cdf-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4cdf-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4cdf-144">JSON representation</span></span>

<span data-ttu-id="d4cdf-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4cdf-145">Here is a JSON representation of the resource.</span></span>

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
