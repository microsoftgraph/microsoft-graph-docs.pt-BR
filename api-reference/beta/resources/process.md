---
title: tipo de recurso Process
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: a024cfbabcff4357427ae6a814da00af83eae304
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070489"
---
# <a name="process-resource-type"></a><span data-ttu-id="bbc5b-104">tipo de recurso Process</span><span class="sxs-lookup"><span data-stu-id="bbc5b-104">process resource type</span></span>

<span data-ttu-id="bbc5b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc5b-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc5b-106">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-106">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="bbc5b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbc5b-107">Properties</span></span>

| <span data-ttu-id="bbc5b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbc5b-108">Property</span></span>   | <span data-ttu-id="bbc5b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbc5b-109">Type</span></span>|<span data-ttu-id="bbc5b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc5b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbc5b-111">accountName</span><span class="sxs-lookup"><span data-stu-id="bbc5b-111">accountName</span></span>|<span data-ttu-id="bbc5b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbc5b-112">String</span></span>|<span data-ttu-id="bbc5b-113">Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-113">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="bbc5b-114">commandLine</span><span class="sxs-lookup"><span data-stu-id="bbc5b-114">commandLine</span></span>|<span data-ttu-id="bbc5b-115">String</span><span class="sxs-lookup"><span data-stu-id="bbc5b-115">String</span></span>|<span data-ttu-id="bbc5b-116">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-116">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="bbc5b-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbc5b-117">createdDateTime</span></span>|<span data-ttu-id="bbc5b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbc5b-118">DateTimeOffset</span></span>|<span data-ttu-id="bbc5b-119">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-119">Time at which the process was started.</span></span> <span data-ttu-id="bbc5b-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbc5b-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bbc5b-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="bbc5b-122">fileHash</span></span>|[<span data-ttu-id="bbc5b-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="bbc5b-123">fileHash</span></span>](filehash.md)|<span data-ttu-id="bbc5b-124">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="bbc5b-124">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="bbc5b-125">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="bbc5b-125">integrityLevel</span></span>|<span data-ttu-id="bbc5b-126">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="bbc5b-126">processIntegrityLevel</span></span>|<span data-ttu-id="bbc5b-127">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-127">The integrity level of the process.</span></span> <span data-ttu-id="bbc5b-128">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-128">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="bbc5b-129">iselevados</span><span class="sxs-lookup"><span data-stu-id="bbc5b-129">isElevated</span></span>|<span data-ttu-id="bbc5b-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbc5b-130">Boolean</span></span>|<span data-ttu-id="bbc5b-131">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-131">True if the process is elevated.</span></span>|
|<span data-ttu-id="bbc5b-132">name</span><span class="sxs-lookup"><span data-stu-id="bbc5b-132">name</span></span>|<span data-ttu-id="bbc5b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbc5b-133">String</span></span>|<span data-ttu-id="bbc5b-134">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-134">The name of the process' Image file.</span></span>|
|<span data-ttu-id="bbc5b-135">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbc5b-135">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="bbc5b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbc5b-136">DateTimeOffset</span></span>|<span data-ttu-id="bbc5b-137">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-137">DateTime at which the parent process was started.</span></span> <span data-ttu-id="bbc5b-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbc5b-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bbc5b-140">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="bbc5b-140">parentProcessId</span></span>|<span data-ttu-id="bbc5b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc5b-141">Int32</span></span>|<span data-ttu-id="bbc5b-142">A ID de processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-142">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="bbc5b-143">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="bbc5b-143">parentProcessName</span></span>|<span data-ttu-id="bbc5b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbc5b-144">String</span></span>|<span data-ttu-id="bbc5b-145">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-145">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="bbc5b-146">caminho</span><span class="sxs-lookup"><span data-stu-id="bbc5b-146">path</span></span>|<span data-ttu-id="bbc5b-147">String</span><span class="sxs-lookup"><span data-stu-id="bbc5b-147">String</span></span>|<span data-ttu-id="bbc5b-148">Caminho completo, incluindo o nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-148">Full path, including filename.</span></span>|
|<span data-ttu-id="bbc5b-149">Identificação</span><span class="sxs-lookup"><span data-stu-id="bbc5b-149">processId</span></span>|<span data-ttu-id="bbc5b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc5b-150">Int32</span></span>|<span data-ttu-id="bbc5b-151">A identificação do processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-151">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbc5b-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbc5b-152">JSON representation</span></span>

<span data-ttu-id="bbc5b-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbc5b-153">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


