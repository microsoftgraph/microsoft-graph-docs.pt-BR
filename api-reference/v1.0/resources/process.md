---
title: tipo de recurso Process
description: Contém informações de estado sobre o processo relacionado ao alerta.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ccaf2e3048fc26573e9599a515aabf391dda6d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035081"
---
# <a name="process-resource-type"></a><span data-ttu-id="1eab1-103">tipo de recurso Process</span><span class="sxs-lookup"><span data-stu-id="1eab1-103">process resource type</span></span>

<span data-ttu-id="1eab1-104">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="1eab1-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1eab1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1eab1-105">Properties</span></span>

| <span data-ttu-id="1eab1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eab1-106">Property</span></span>   | <span data-ttu-id="1eab1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eab1-107">Type</span></span>|<span data-ttu-id="1eab1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eab1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eab1-109">accountName</span><span class="sxs-lookup"><span data-stu-id="1eab1-109">accountName</span></span>|<span data-ttu-id="1eab1-110">String</span><span class="sxs-lookup"><span data-stu-id="1eab1-110">String</span></span>|<span data-ttu-id="1eab1-111">Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="1eab1-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="1eab1-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="1eab1-112">commandLine</span></span>|<span data-ttu-id="1eab1-113">String</span><span class="sxs-lookup"><span data-stu-id="1eab1-113">String</span></span>|<span data-ttu-id="1eab1-114">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1eab1-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="1eab1-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1eab1-115">createdDateTime</span></span>|<span data-ttu-id="1eab1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1eab1-116">DateTimeOffset</span></span>|<span data-ttu-id="1eab1-117">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="1eab1-117">Time at which the process was started.</span></span> <span data-ttu-id="1eab1-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1eab1-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1eab1-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1eab1-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1eab1-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="1eab1-120">fileHash</span></span>|[<span data-ttu-id="1eab1-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="1eab1-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="1eab1-122">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="1eab1-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="1eab1-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="1eab1-123">integrityLevel</span></span>|<span data-ttu-id="1eab1-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="1eab1-124">processIntegrityLevel</span></span>|<span data-ttu-id="1eab1-125">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="1eab1-125">The integrity level of the process.</span></span> <span data-ttu-id="1eab1-126">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="1eab1-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="1eab1-127">iselevados</span><span class="sxs-lookup"><span data-stu-id="1eab1-127">isElevated</span></span>|<span data-ttu-id="1eab1-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="1eab1-128">Boolean</span></span>|<span data-ttu-id="1eab1-129">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="1eab1-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="1eab1-130">name</span><span class="sxs-lookup"><span data-stu-id="1eab1-130">name</span></span>|<span data-ttu-id="1eab1-131">String</span><span class="sxs-lookup"><span data-stu-id="1eab1-131">String</span></span>|<span data-ttu-id="1eab1-132">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="1eab1-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="1eab1-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1eab1-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="1eab1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1eab1-134">DateTimeOffset</span></span>|<span data-ttu-id="1eab1-135">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="1eab1-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="1eab1-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1eab1-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1eab1-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1eab1-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1eab1-138">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="1eab1-138">parentProcessId</span></span>|<span data-ttu-id="1eab1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1eab1-139">Int32</span></span>|<span data-ttu-id="1eab1-140">A ID de processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="1eab1-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="1eab1-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="1eab1-141">parentProcessName</span></span>|<span data-ttu-id="1eab1-142">String</span><span class="sxs-lookup"><span data-stu-id="1eab1-142">String</span></span>|<span data-ttu-id="1eab1-143">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="1eab1-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="1eab1-144">caminho</span><span class="sxs-lookup"><span data-stu-id="1eab1-144">path</span></span>|<span data-ttu-id="1eab1-145">String</span><span class="sxs-lookup"><span data-stu-id="1eab1-145">String</span></span>|<span data-ttu-id="1eab1-146">Caminho completo, incluindo o nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1eab1-146">Full path, including filename.</span></span>|
|<span data-ttu-id="1eab1-147">Identificação</span><span class="sxs-lookup"><span data-stu-id="1eab1-147">processId</span></span>|<span data-ttu-id="1eab1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1eab1-148">Int32</span></span>|<span data-ttu-id="1eab1-149">A identificação do processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="1eab1-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1eab1-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1eab1-150">JSON representation</span></span>

<span data-ttu-id="1eab1-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1eab1-151">The following is a JSON representation of the resource.</span></span>

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
