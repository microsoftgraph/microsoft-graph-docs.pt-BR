---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bacdcc3c2ec7368597a03d40e6835f09e02cd7f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018778"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="e19a0-105">tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e19a0-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="e19a0-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e19a0-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e19a0-107">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="e19a0-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="e19a0-108">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="e19a0-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="e19a0-109">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="e19a0-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="e19a0-110">Methods</span><span class="sxs-lookup"><span data-stu-id="e19a0-110">Methods</span></span>

| <span data-ttu-id="e19a0-111">Método</span><span class="sxs-lookup"><span data-stu-id="e19a0-111">Method</span></span>           | <span data-ttu-id="e19a0-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e19a0-112">Return Type</span></span>    |<span data-ttu-id="e19a0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e19a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e19a0-114">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e19a0-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="e19a0-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e19a0-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="e19a0-116">Recupere as propriedades do objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="e19a0-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="e19a0-117">Exportar dados pessoais</span><span class="sxs-lookup"><span data-stu-id="e19a0-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="e19a0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e19a0-118">None</span></span> |<span data-ttu-id="e19a0-119">Enviar uma solicitação de operação de política de dados para exportar dados do usuário organizacional que podem ser lidas novamente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="e19a0-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="e19a0-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e19a0-120">Properties</span></span>

> <span data-ttu-id="e19a0-121">**Observação:** Todas as propriedades deste recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e19a0-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="e19a0-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e19a0-122">Property</span></span>     | <span data-ttu-id="e19a0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e19a0-123">Type</span></span>   |<span data-ttu-id="e19a0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e19a0-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e19a0-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e19a0-125">completedDateTime</span></span>|<span data-ttu-id="e19a0-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e19a0-126">DateTimeOffset</span></span>|<span data-ttu-id="e19a0-127">Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e19a0-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e19a0-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e19a0-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e19a0-129">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="e19a0-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="e19a0-130">id</span><span class="sxs-lookup"><span data-stu-id="e19a0-130">id</span></span>|<span data-ttu-id="e19a0-131">String</span><span class="sxs-lookup"><span data-stu-id="e19a0-131">String</span></span>| <span data-ttu-id="e19a0-132">Chave exclusiva para esta operação.</span><span class="sxs-lookup"><span data-stu-id="e19a0-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="e19a0-133">status</span><span class="sxs-lookup"><span data-stu-id="e19a0-133">status</span></span>|<span data-ttu-id="e19a0-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e19a0-134">string</span></span>| <span data-ttu-id="e19a0-135">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e19a0-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e19a0-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="e19a0-136">storageLocation</span></span>|<span data-ttu-id="e19a0-137">String</span><span class="sxs-lookup"><span data-stu-id="e19a0-137">String</span></span>|<span data-ttu-id="e19a0-138">O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="e19a0-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="e19a0-139">userId</span><span class="sxs-lookup"><span data-stu-id="e19a0-139">userId</span></span>|<span data-ttu-id="e19a0-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e19a0-140">String</span></span>|<span data-ttu-id="e19a0-141">A ID do usuário em que a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="e19a0-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="e19a0-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="e19a0-142">submittedDateTime</span></span>|<span data-ttu-id="e19a0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e19a0-143">DateTimeOffset</span></span>|<span data-ttu-id="e19a0-144">Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e19a0-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e19a0-145">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e19a0-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e19a0-146">progresso</span><span class="sxs-lookup"><span data-stu-id="e19a0-146">progress</span></span>|<span data-ttu-id="e19a0-147">String</span><span class="sxs-lookup"><span data-stu-id="e19a0-147">String</span></span>|<span data-ttu-id="e19a0-148">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="e19a0-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e19a0-149">Relações</span><span class="sxs-lookup"><span data-stu-id="e19a0-149">Relationships</span></span>
<span data-ttu-id="e19a0-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e19a0-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e19a0-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e19a0-151">JSON representation</span></span>

<span data-ttu-id="e19a0-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e19a0-152">The following is a JSON representation of the resource.</span></span>

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

