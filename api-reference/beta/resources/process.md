---
title: tipo de recurso do processo
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 2e60c9e008ccfddaa0bcc3e78c27cc17c65a3844
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036374"
---
# <a name="process-resource-type"></a><span data-ttu-id="601a9-104">tipo de recurso do processo</span><span class="sxs-lookup"><span data-stu-id="601a9-104">process resource type</span></span>

 > <span data-ttu-id="601a9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="601a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="601a9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="601a9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="601a9-107">Contém informações com informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="601a9-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="601a9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="601a9-108">Properties</span></span>

| <span data-ttu-id="601a9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="601a9-109">Property</span></span>   | <span data-ttu-id="601a9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="601a9-110">Type</span></span>|<span data-ttu-id="601a9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="601a9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="601a9-112">accountName</span><span class="sxs-lookup"><span data-stu-id="601a9-112">accountName</span></span>|<span data-ttu-id="601a9-113">String</span><span class="sxs-lookup"><span data-stu-id="601a9-113">String</span></span>|<span data-ttu-id="601a9-114">Identificador (o contexto de conta do usuário o processo eram executado em) de conta de usuário de exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="601a9-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="601a9-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="601a9-115">commandLine</span></span>|<span data-ttu-id="601a9-116">String</span><span class="sxs-lookup"><span data-stu-id="601a9-116">String</span></span>|<span data-ttu-id="601a9-117">A commandline de invocação do processo completo incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="601a9-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="601a9-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="601a9-118">createdDateTime</span></span>|<span data-ttu-id="601a9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="601a9-119">DateTimeOffset</span></span>|<span data-ttu-id="601a9-120">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="601a9-120">Time at which the process was started.</span></span> <span data-ttu-id="601a9-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="601a9-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="601a9-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="601a9-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="601a9-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="601a9-123">fileHash</span></span>|[<span data-ttu-id="601a9-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="601a9-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="601a9-125">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="601a9-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="601a9-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="601a9-126">integrityLevel</span></span>|<span data-ttu-id="601a9-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="601a9-127">processIntegrityLevel</span></span>|<span data-ttu-id="601a9-128">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="601a9-128">The integrity level of the process.</span></span> <span data-ttu-id="601a9-129">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="601a9-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="601a9-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="601a9-130">isElevated</span></span>|<span data-ttu-id="601a9-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="601a9-131">Boolean</span></span>|<span data-ttu-id="601a9-132">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="601a9-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="601a9-133">name</span><span class="sxs-lookup"><span data-stu-id="601a9-133">name</span></span>|<span data-ttu-id="601a9-134">String</span><span class="sxs-lookup"><span data-stu-id="601a9-134">String</span></span>|<span data-ttu-id="601a9-135">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="601a9-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="601a9-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="601a9-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="601a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="601a9-137">DateTimeOffset</span></span>|<span data-ttu-id="601a9-138">Data e hora em que o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="601a9-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="601a9-139">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="601a9-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="601a9-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="601a9-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="601a9-141">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="601a9-141">parentProcessId</span></span>|<span data-ttu-id="601a9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="601a9-142">Int32</span></span>|<span data-ttu-id="601a9-143">O processo de identificação do processo pai.</span><span class="sxs-lookup"><span data-stu-id="601a9-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="601a9-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="601a9-144">parentProcessName</span></span>|<span data-ttu-id="601a9-145">String</span><span class="sxs-lookup"><span data-stu-id="601a9-145">String</span></span>|<span data-ttu-id="601a9-146">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="601a9-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="601a9-147">caminho</span><span class="sxs-lookup"><span data-stu-id="601a9-147">path</span></span>|<span data-ttu-id="601a9-148">String</span><span class="sxs-lookup"><span data-stu-id="601a9-148">String</span></span>|<span data-ttu-id="601a9-149">Caminho completo, incluindo nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="601a9-149">Full path, including filename.</span></span>|
|<span data-ttu-id="601a9-150">processId</span><span class="sxs-lookup"><span data-stu-id="601a9-150">processId</span></span>|<span data-ttu-id="601a9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="601a9-151">Int32</span></span>|<span data-ttu-id="601a9-152">O processo de identificação do processo.</span><span class="sxs-lookup"><span data-stu-id="601a9-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="601a9-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="601a9-153">JSON representation</span></span>

<span data-ttu-id="601a9-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="601a9-154">The following is a JSON representation of the resource.</span></span>

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