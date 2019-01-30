---
title: tipo de recurso de dataPolicyOperation
description: Representa uma operação de diretiva de dados enviados. Ele contém as informações necessárias para rastrear o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d3ec392bb30614346d2726262851eebc29ee779
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643990"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="cd6aa-105">tipo de recurso de dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="cd6aa-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="cd6aa-106">Representa uma operação de diretiva de dados enviados.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="cd6aa-107">Ele contém as informações necessárias para rastrear o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="cd6aa-108">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="cd6aa-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd6aa-109">Methods</span></span>

| <span data-ttu-id="cd6aa-110">Método</span><span class="sxs-lookup"><span data-stu-id="cd6aa-110">Method</span></span>           | <span data-ttu-id="cd6aa-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd6aa-111">Return Type</span></span>    |<span data-ttu-id="cd6aa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6aa-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd6aa-113">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="cd6aa-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="cd6aa-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="cd6aa-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="cd6aa-115">Leia as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd6aa-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd6aa-116">Properties</span></span>

> <span data-ttu-id="cd6aa-117">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="cd6aa-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd6aa-118">Property</span></span>     | <span data-ttu-id="cd6aa-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd6aa-119">Type</span></span>   |<span data-ttu-id="cd6aa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6aa-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd6aa-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6aa-121">completedDateTime</span></span>|<span data-ttu-id="cd6aa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6aa-122">DateTimeOffset</span></span>|<span data-ttu-id="cd6aa-123">Representa quando a solicitação para esta operação de política de dados foi concluída, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="cd6aa-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cd6aa-125">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="cd6aa-126">id</span><span class="sxs-lookup"><span data-stu-id="cd6aa-126">id</span></span>|<span data-ttu-id="cd6aa-127">String</span><span class="sxs-lookup"><span data-stu-id="cd6aa-127">String</span></span>| <span data-ttu-id="cd6aa-128">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="cd6aa-129">status</span><span class="sxs-lookup"><span data-stu-id="cd6aa-129">status</span></span>|<span data-ttu-id="cd6aa-130">string</span><span class="sxs-lookup"><span data-stu-id="cd6aa-130">string</span></span>| <span data-ttu-id="cd6aa-131">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cd6aa-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="cd6aa-132">storageLocation</span></span>|<span data-ttu-id="cd6aa-133">String</span><span class="sxs-lookup"><span data-stu-id="cd6aa-133">String</span></span>|<span data-ttu-id="cd6aa-134">O local da URL para onde os dados está sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="cd6aa-135">userId</span><span class="sxs-lookup"><span data-stu-id="cd6aa-135">userId</span></span>|<span data-ttu-id="cd6aa-136">String</span><span class="sxs-lookup"><span data-stu-id="cd6aa-136">String</span></span>|<span data-ttu-id="cd6aa-137">A identificação do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="cd6aa-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6aa-138">submittedDateTime</span></span>|<span data-ttu-id="cd6aa-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6aa-139">DateTimeOffset</span></span>|<span data-ttu-id="cd6aa-140">Representa quando a solicitação para esta operação de dados foi enviada, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="cd6aa-141">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cd6aa-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cd6aa-142">progresso</span><span class="sxs-lookup"><span data-stu-id="cd6aa-142">progress</span></span>|<span data-ttu-id="cd6aa-143">Duplo</span><span class="sxs-lookup"><span data-stu-id="cd6aa-143">Double</span></span>|<span data-ttu-id="cd6aa-144">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd6aa-145">Relações</span><span class="sxs-lookup"><span data-stu-id="cd6aa-145">Relationships</span></span>
<span data-ttu-id="cd6aa-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd6aa-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cd6aa-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd6aa-147">JSON representation</span></span>

<span data-ttu-id="cd6aa-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd6aa-148">Here is a JSON representation of the resource.</span></span>

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
