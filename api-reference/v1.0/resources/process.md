---
title: tipo de recurso de processo
description: Contém informações de estado sobre o processo relacionado ao alerta.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d29a09b2d593fcf1c4a3cb5bee4230e57e9836d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720727"
---
# <a name="process-resource-type"></a><span data-ttu-id="fe4fc-103">tipo de recurso de processo</span><span class="sxs-lookup"><span data-stu-id="fe4fc-103">process resource type</span></span>

<span data-ttu-id="fe4fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe4fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe4fc-105">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="fe4fc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe4fc-106">Properties</span></span>

| <span data-ttu-id="fe4fc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe4fc-107">Property</span></span>   | <span data-ttu-id="fe4fc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe4fc-108">Type</span></span>|<span data-ttu-id="fe4fc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe4fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe4fc-110">accountName</span><span class="sxs-lookup"><span data-stu-id="fe4fc-110">accountName</span></span>|<span data-ttu-id="fe4fc-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe4fc-111">String</span></span>|<span data-ttu-id="fe4fc-112">Identificador de conta de usuário (contexto de conta de usuário no qual o processo foi submetido) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="fe4fc-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="fe4fc-113">commandLine</span></span>|<span data-ttu-id="fe4fc-114">String</span><span class="sxs-lookup"><span data-stu-id="fe4fc-114">String</span></span>|<span data-ttu-id="fe4fc-115">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="fe4fc-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe4fc-116">createdDateTime</span></span>|<span data-ttu-id="fe4fc-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe4fc-117">DateTimeOffset</span></span>|<span data-ttu-id="fe4fc-118">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-118">Time at which the process was started.</span></span> <span data-ttu-id="fe4fc-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe4fc-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fe4fc-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="fe4fc-121">fileHash</span></span>|[<span data-ttu-id="fe4fc-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="fe4fc-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="fe4fc-123">Tipo complexo que contém hashes de arquivo (criptográficos e sensíveis ao local).</span><span class="sxs-lookup"><span data-stu-id="fe4fc-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="fe4fc-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="fe4fc-124">integrityLevel</span></span>|<span data-ttu-id="fe4fc-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="fe4fc-125">processIntegrityLevel</span></span>|<span data-ttu-id="fe4fc-126">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-126">The integrity level of the process.</span></span> <span data-ttu-id="fe4fc-127">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="fe4fc-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="fe4fc-128">isElevated</span></span>|<span data-ttu-id="fe4fc-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe4fc-129">Boolean</span></span>|<span data-ttu-id="fe4fc-130">True se o processo estiver elevado.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="fe4fc-131">nome</span><span class="sxs-lookup"><span data-stu-id="fe4fc-131">name</span></span>|<span data-ttu-id="fe4fc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe4fc-132">String</span></span>|<span data-ttu-id="fe4fc-133">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="fe4fc-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe4fc-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="fe4fc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe4fc-135">DateTimeOffset</span></span>|<span data-ttu-id="fe4fc-136">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="fe4fc-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe4fc-138">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fe4fc-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="fe4fc-139">parentProcessId</span></span>|<span data-ttu-id="fe4fc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4fc-140">Int32</span></span>|<span data-ttu-id="fe4fc-141">A ID do Processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="fe4fc-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="fe4fc-142">parentProcessName</span></span>|<span data-ttu-id="fe4fc-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe4fc-143">String</span></span>|<span data-ttu-id="fe4fc-144">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="fe4fc-145">caminho</span><span class="sxs-lookup"><span data-stu-id="fe4fc-145">path</span></span>|<span data-ttu-id="fe4fc-146">String</span><span class="sxs-lookup"><span data-stu-id="fe4fc-146">String</span></span>|<span data-ttu-id="fe4fc-147">Caminho completo, incluindo nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-147">Full path, including filename.</span></span>|
|<span data-ttu-id="fe4fc-148">processId</span><span class="sxs-lookup"><span data-stu-id="fe4fc-148">processId</span></span>|<span data-ttu-id="fe4fc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fe4fc-149">Int32</span></span>|<span data-ttu-id="fe4fc-150">A ID do Processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe4fc-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe4fc-151">JSON representation</span></span>

<span data-ttu-id="fe4fc-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe4fc-152">The following is a JSON representation of the resource.</span></span>

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

