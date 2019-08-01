---
title: tipo de recurso dataPolicyOperation
description: Representa uma operação de política de dados enviada. Ele contém informações necessárias para controlar o status de uma operação. Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c73bef8a640c950b6d85eb74ad93089aaad4f74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029551"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="1dd4f-105">tipo de recurso dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1dd4f-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="1dd4f-106">Representa uma operação de política de dados enviada.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="1dd4f-107">Ele contém informações necessárias para controlar o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="1dd4f-108">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, posteriormente, rastrear essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="1dd4f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="1dd4f-109">Methods</span></span>

| <span data-ttu-id="1dd4f-110">Método</span><span class="sxs-lookup"><span data-stu-id="1dd4f-110">Method</span></span>           | <span data-ttu-id="1dd4f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1dd4f-111">Return Type</span></span>    |<span data-ttu-id="1dd4f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd4f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1dd4f-113">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1dd4f-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="1dd4f-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1dd4f-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="1dd4f-115">Recupere as propriedades do objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="1dd4f-115">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="1dd4f-116">Exportar dados pessoais</span><span class="sxs-lookup"><span data-stu-id="1dd4f-116">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="1dd4f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dd4f-117">None</span></span> |<span data-ttu-id="1dd4f-118">Enviar uma solicitação de operação de política de dados para exportar dados do usuário organizacional que podem ser lidas novamente usando [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="1dd4f-118">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="1dd4f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dd4f-119">Properties</span></span>

> <span data-ttu-id="1dd4f-120">**Observação:** Todas as propriedades deste recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-120">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="1dd4f-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dd4f-121">Property</span></span>     | <span data-ttu-id="1dd4f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dd4f-122">Type</span></span>   |<span data-ttu-id="1dd4f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd4f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd4f-124">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd4f-124">completedDateTime</span></span>|<span data-ttu-id="1dd4f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd4f-125">DateTimeOffset</span></span>|<span data-ttu-id="1dd4f-126">Representa quando a solicitação para esta operação de política de dados foi concluída, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-126">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="1dd4f-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1dd4f-128">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-128">Null until the operation completes.</span></span>|
|<span data-ttu-id="1dd4f-129">id</span><span class="sxs-lookup"><span data-stu-id="1dd4f-129">id</span></span>|<span data-ttu-id="1dd4f-130">String</span><span class="sxs-lookup"><span data-stu-id="1dd4f-130">String</span></span>| <span data-ttu-id="1dd4f-131">Chave exclusiva para esta operação.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-131">Unique key for this operation.</span></span> |
|<span data-ttu-id="1dd4f-132">status</span><span class="sxs-lookup"><span data-stu-id="1dd4f-132">status</span></span>|<span data-ttu-id="1dd4f-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dd4f-133">string</span></span>| <span data-ttu-id="1dd4f-134">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-134">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1dd4f-135">storageLocation</span><span class="sxs-lookup"><span data-stu-id="1dd4f-135">storageLocation</span></span>|<span data-ttu-id="1dd4f-136">String</span><span class="sxs-lookup"><span data-stu-id="1dd4f-136">String</span></span>|<span data-ttu-id="1dd4f-137">O local da URL para o qual os dados estão sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-137">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="1dd4f-138">userId</span><span class="sxs-lookup"><span data-stu-id="1dd4f-138">userId</span></span>|<span data-ttu-id="1dd4f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dd4f-139">String</span></span>|<span data-ttu-id="1dd4f-140">A ID do usuário em que a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-140">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="1dd4f-141">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd4f-141">submittedDateTime</span></span>|<span data-ttu-id="1dd4f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd4f-142">DateTimeOffset</span></span>|<span data-ttu-id="1dd4f-143">Representa quando a solicitação para esta operação de dados foi enviada, em horário UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-143">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="1dd4f-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1dd4f-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1dd4f-145">progresso</span><span class="sxs-lookup"><span data-stu-id="1dd4f-145">progress</span></span>|<span data-ttu-id="1dd4f-146">String</span><span class="sxs-lookup"><span data-stu-id="1dd4f-146">String</span></span>|<span data-ttu-id="1dd4f-147">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-147">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dd4f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="1dd4f-148">Relationships</span></span>
<span data-ttu-id="1dd4f-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dd4f-149">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1dd4f-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dd4f-150">JSON representation</span></span>

<span data-ttu-id="1dd4f-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dd4f-151">The following is a JSON representation of the resource.</span></span>

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
