---
title: tipo de recurso do processo
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869465"
---
# <a name="process-resource-type"></a><span data-ttu-id="41053-104">tipo de recurso do processo</span><span class="sxs-lookup"><span data-stu-id="41053-104">process resource type</span></span>

 > <span data-ttu-id="41053-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41053-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41053-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41053-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41053-107">Contém informações com informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="41053-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="41053-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41053-108">Properties</span></span>

| <span data-ttu-id="41053-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41053-109">Property</span></span>   | <span data-ttu-id="41053-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41053-110">Type</span></span>|<span data-ttu-id="41053-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41053-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41053-112">accountName</span><span class="sxs-lookup"><span data-stu-id="41053-112">accountName</span></span>|<span data-ttu-id="41053-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41053-113">String</span></span>|<span data-ttu-id="41053-114">Identificador (o contexto de conta do usuário o processo eram executado em) de conta de usuário de exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="41053-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="41053-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="41053-115">commandLine</span></span>|<span data-ttu-id="41053-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41053-116">String</span></span>|<span data-ttu-id="41053-117">A commandline de invocação do processo completo incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="41053-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="41053-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41053-118">createdDateTime</span></span>|<span data-ttu-id="41053-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41053-119">DateTimeOffset</span></span>|<span data-ttu-id="41053-120">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="41053-120">Time at which the process was started.</span></span> <span data-ttu-id="41053-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41053-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41053-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="41053-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="41053-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="41053-123">fileHash</span></span>|[<span data-ttu-id="41053-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="41053-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="41053-125">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="41053-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="41053-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="41053-126">integrityLevel</span></span>|<span data-ttu-id="41053-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="41053-127">processIntegrityLevel</span></span>|<span data-ttu-id="41053-128">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="41053-128">The integrity level of the process.</span></span> <span data-ttu-id="41053-129">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="41053-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="41053-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="41053-130">isElevated</span></span>|<span data-ttu-id="41053-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="41053-131">Boolean</span></span>|<span data-ttu-id="41053-132">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="41053-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="41053-133">name</span><span class="sxs-lookup"><span data-stu-id="41053-133">name</span></span>|<span data-ttu-id="41053-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41053-134">String</span></span>|<span data-ttu-id="41053-135">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="41053-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="41053-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="41053-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="41053-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41053-137">DateTimeOffset</span></span>|<span data-ttu-id="41053-138">Data e hora em que o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="41053-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="41053-139">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41053-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41053-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="41053-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="41053-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="41053-141">parentProcessId</span></span>|<span data-ttu-id="41053-142">Int32</span><span class="sxs-lookup"><span data-stu-id="41053-142">Int32</span></span>|<span data-ttu-id="41053-143">O processo de identificação do processo pai.</span><span class="sxs-lookup"><span data-stu-id="41053-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="41053-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="41053-144">parentProcessName</span></span>|<span data-ttu-id="41053-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41053-145">String</span></span>|<span data-ttu-id="41053-146">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="41053-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="41053-147">caminho</span><span class="sxs-lookup"><span data-stu-id="41053-147">path</span></span>|<span data-ttu-id="41053-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41053-148">String</span></span>|<span data-ttu-id="41053-149">Caminho completo, incluindo nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="41053-149">Full path, including filename.</span></span>|
|<span data-ttu-id="41053-150">processId</span><span class="sxs-lookup"><span data-stu-id="41053-150">processId</span></span>|<span data-ttu-id="41053-151">Int32</span><span class="sxs-lookup"><span data-stu-id="41053-151">Int32</span></span>|<span data-ttu-id="41053-152">O processo de identificação do processo.</span><span class="sxs-lookup"><span data-stu-id="41053-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41053-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41053-153">JSON representation</span></span>

<span data-ttu-id="41053-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41053-154">The following is a JSON representation of the resource.</span></span>

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
