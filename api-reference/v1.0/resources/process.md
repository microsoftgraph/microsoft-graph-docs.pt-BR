---
title: tipo de recurso Process
description: Contém informações de estado sobre o processo relacionado ao alerta.
localization_priority: Normal
ms.openlocfilehash: 0b4207c1780dfd6327ceb67e837f793341e609ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579871"
---
# <a name="process-resource-type"></a><span data-ttu-id="be395-103">tipo de recurso Process</span><span class="sxs-lookup"><span data-stu-id="be395-103">process resource type</span></span>

<span data-ttu-id="be395-104">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="be395-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="be395-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be395-105">Properties</span></span>

| <span data-ttu-id="be395-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be395-106">Property</span></span>   | <span data-ttu-id="be395-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="be395-107">Type</span></span>|<span data-ttu-id="be395-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="be395-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be395-109">accountName</span><span class="sxs-lookup"><span data-stu-id="be395-109">accountName</span></span>|<span data-ttu-id="be395-110">String</span><span class="sxs-lookup"><span data-stu-id="be395-110">String</span></span>|<span data-ttu-id="be395-111">Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="be395-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="be395-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="be395-112">commandLine</span></span>|<span data-ttu-id="be395-113">String</span><span class="sxs-lookup"><span data-stu-id="be395-113">String</span></span>|<span data-ttu-id="be395-114">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="be395-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="be395-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be395-115">createdDateTime</span></span>|<span data-ttu-id="be395-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be395-116">DateTimeOffset</span></span>|<span data-ttu-id="be395-117">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="be395-117">Time at which the process was started.</span></span> <span data-ttu-id="be395-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="be395-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="be395-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="be395-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="be395-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="be395-120">fileHash</span></span>|[<span data-ttu-id="be395-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="be395-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="be395-122">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="be395-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="be395-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="be395-123">integrityLevel</span></span>|<span data-ttu-id="be395-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="be395-124">processIntegrityLevel</span></span>|<span data-ttu-id="be395-125">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="be395-125">The integrity level of the process.</span></span> <span data-ttu-id="be395-126">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="be395-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="be395-127">isElevados</span><span class="sxs-lookup"><span data-stu-id="be395-127">isElevated</span></span>|<span data-ttu-id="be395-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="be395-128">Boolean</span></span>|<span data-ttu-id="be395-129">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="be395-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="be395-130">name</span><span class="sxs-lookup"><span data-stu-id="be395-130">name</span></span>|<span data-ttu-id="be395-131">String</span><span class="sxs-lookup"><span data-stu-id="be395-131">String</span></span>|<span data-ttu-id="be395-132">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="be395-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="be395-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="be395-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="be395-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be395-134">DateTimeOffset</span></span>|<span data-ttu-id="be395-135">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="be395-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="be395-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="be395-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="be395-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="be395-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="be395-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="be395-138">parentProcessId</span></span>|<span data-ttu-id="be395-139">Int32</span><span class="sxs-lookup"><span data-stu-id="be395-139">Int32</span></span>|<span data-ttu-id="be395-140">A ID de processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="be395-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="be395-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="be395-141">parentProcessName</span></span>|<span data-ttu-id="be395-142">String</span><span class="sxs-lookup"><span data-stu-id="be395-142">String</span></span>|<span data-ttu-id="be395-143">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="be395-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="be395-144">caminho</span><span class="sxs-lookup"><span data-stu-id="be395-144">path</span></span>|<span data-ttu-id="be395-145">String</span><span class="sxs-lookup"><span data-stu-id="be395-145">String</span></span>|<span data-ttu-id="be395-146">Caminho completo, incluindo o nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="be395-146">Full path, including filename.</span></span>|
|<span data-ttu-id="be395-147">Identificação</span><span class="sxs-lookup"><span data-stu-id="be395-147">processId</span></span>|<span data-ttu-id="be395-148">Int32</span><span class="sxs-lookup"><span data-stu-id="be395-148">Int32</span></span>|<span data-ttu-id="be395-149">A identificação do processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="be395-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be395-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be395-150">JSON representation</span></span>

<span data-ttu-id="be395-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be395-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
