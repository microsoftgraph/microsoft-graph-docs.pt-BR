---
title: Tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 27843a57190910584bcc09c4f65aa75314e3ab1c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449009"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="b277b-105">Tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b277b-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="b277b-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b277b-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b277b-107">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="b277b-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="b277b-108">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="b277b-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="b277b-109">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar dados da empresa de um funcionário e, em seguida, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="b277b-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="b277b-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="b277b-110">Methods</span></span>

| <span data-ttu-id="b277b-111">Método</span><span class="sxs-lookup"><span data-stu-id="b277b-111">Method</span></span>           | <span data-ttu-id="b277b-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b277b-112">Return Type</span></span>    |<span data-ttu-id="b277b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b277b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b277b-114">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b277b-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="b277b-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b277b-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="b277b-116">Recupere propriedades do **objeto dataPolicyOperation.**</span><span class="sxs-lookup"><span data-stu-id="b277b-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="b277b-117">Exportar dados pessoais</span><span class="sxs-lookup"><span data-stu-id="b277b-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="b277b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b277b-118">None</span></span> |<span data-ttu-id="b277b-119">Enviar uma solicitação de operação de política de dados para exportar os dados do usuário organizacional que podem ser lidos posteriormente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="b277b-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="b277b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b277b-120">Properties</span></span>

> <span data-ttu-id="b277b-121">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b277b-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="b277b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b277b-122">Property</span></span>     | <span data-ttu-id="b277b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b277b-123">Type</span></span>   |<span data-ttu-id="b277b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b277b-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b277b-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b277b-125">completedDateTime</span></span>|<span data-ttu-id="b277b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b277b-126">DateTimeOffset</span></span>|<span data-ttu-id="b277b-127">Representa quando a solicitação para essa operação de política de dados foi concluída, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="b277b-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="b277b-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b277b-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b277b-129">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="b277b-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="b277b-130">id</span><span class="sxs-lookup"><span data-stu-id="b277b-130">id</span></span>|<span data-ttu-id="b277b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b277b-131">String</span></span>| <span data-ttu-id="b277b-132">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="b277b-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="b277b-133">status</span><span class="sxs-lookup"><span data-stu-id="b277b-133">status</span></span>|<span data-ttu-id="b277b-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b277b-134">string</span></span>| <span data-ttu-id="b277b-135">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b277b-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b277b-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="b277b-136">storageLocation</span></span>|<span data-ttu-id="b277b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b277b-137">String</span></span>|<span data-ttu-id="b277b-138">O local da URL para onde os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="b277b-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="b277b-139">userId</span><span class="sxs-lookup"><span data-stu-id="b277b-139">userId</span></span>|<span data-ttu-id="b277b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b277b-140">String</span></span>|<span data-ttu-id="b277b-141">A id do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="b277b-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="b277b-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="b277b-142">submittedDateTime</span></span>|<span data-ttu-id="b277b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b277b-143">DateTimeOffset</span></span>|<span data-ttu-id="b277b-144">Representa quando a solicitação para essa operação de dados foi enviada, em tempo UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="b277b-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="b277b-145">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b277b-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b277b-146">progresso</span><span class="sxs-lookup"><span data-stu-id="b277b-146">progress</span></span>|<span data-ttu-id="b277b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b277b-147">String</span></span>|<span data-ttu-id="b277b-148">Especifica o andamento de uma operação.</span><span class="sxs-lookup"><span data-stu-id="b277b-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b277b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="b277b-149">Relationships</span></span>
<span data-ttu-id="b277b-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b277b-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b277b-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b277b-151">JSON representation</span></span>

<span data-ttu-id="b277b-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b277b-152">The following is a JSON representation of the resource.</span></span>

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

