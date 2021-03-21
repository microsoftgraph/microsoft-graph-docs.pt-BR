---
title: Tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7b07cb2906eb1a3d01d6c24ca5b91fec35ec7c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961997"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="a854c-105">Tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="a854c-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="a854c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a854c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a854c-107">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="a854c-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="a854c-108">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="a854c-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="a854c-109">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="a854c-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="a854c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="a854c-110">Methods</span></span>

| <span data-ttu-id="a854c-111">Método</span><span class="sxs-lookup"><span data-stu-id="a854c-111">Method</span></span>           | <span data-ttu-id="a854c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a854c-112">Return Type</span></span>    |<span data-ttu-id="a854c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a854c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a854c-114">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="a854c-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="a854c-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="a854c-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="a854c-116">Recupere propriedades do **objeto dataPolicyOperation.**</span><span class="sxs-lookup"><span data-stu-id="a854c-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="a854c-117">Exportar dados pessoais</span><span class="sxs-lookup"><span data-stu-id="a854c-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="a854c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a854c-118">None</span></span> |<span data-ttu-id="a854c-119">Enviar uma solicitação de operação de política de dados para exportar os dados do usuário organizacional que podem ser lidos posteriormente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="a854c-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="a854c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a854c-120">Properties</span></span>

> <span data-ttu-id="a854c-121">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a854c-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="a854c-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a854c-122">Property</span></span>     | <span data-ttu-id="a854c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a854c-123">Type</span></span>   |<span data-ttu-id="a854c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a854c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a854c-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="a854c-125">completedDateTime</span></span>|<span data-ttu-id="a854c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a854c-126">DateTimeOffset</span></span>|<span data-ttu-id="a854c-127">Representa quando a solicitação para essa operação de política de dados foi concluída, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="a854c-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="a854c-128">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a854c-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a854c-129">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="a854c-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="a854c-130">id</span><span class="sxs-lookup"><span data-stu-id="a854c-130">id</span></span>|<span data-ttu-id="a854c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a854c-131">String</span></span>| <span data-ttu-id="a854c-132">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="a854c-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="a854c-133">status</span><span class="sxs-lookup"><span data-stu-id="a854c-133">status</span></span>|<span data-ttu-id="a854c-134">dataPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="a854c-134">dataPolicyOperationStatus</span></span>| <span data-ttu-id="a854c-135">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a854c-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a854c-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="a854c-136">storageLocation</span></span>|<span data-ttu-id="a854c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a854c-137">String</span></span>|<span data-ttu-id="a854c-138">O local da URL para onde os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="a854c-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="a854c-139">userId</span><span class="sxs-lookup"><span data-stu-id="a854c-139">userId</span></span>|<span data-ttu-id="a854c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a854c-140">String</span></span>|<span data-ttu-id="a854c-141">A id do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="a854c-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="a854c-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="a854c-142">submittedDateTime</span></span>|<span data-ttu-id="a854c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a854c-143">DateTimeOffset</span></span>|<span data-ttu-id="a854c-144">Representa quando a solicitação para essa operação de dados foi enviada, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="a854c-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="a854c-145">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a854c-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a854c-146">progresso</span><span class="sxs-lookup"><span data-stu-id="a854c-146">progress</span></span>|<span data-ttu-id="a854c-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a854c-147">String</span></span>|<span data-ttu-id="a854c-148">Especifica o andamento de uma operação.</span><span class="sxs-lookup"><span data-stu-id="a854c-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a854c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="a854c-149">Relationships</span></span>
<span data-ttu-id="a854c-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a854c-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a854c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a854c-151">JSON representation</span></span>

<span data-ttu-id="a854c-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a854c-152">The following is a JSON representation of the resource.</span></span>

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
  "progress": "String (double)"
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

