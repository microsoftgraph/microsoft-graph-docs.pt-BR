---
title: tipo de recurso do processo
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521205"
---
# <a name="process-resource-type"></a><span data-ttu-id="8ee14-104">tipo de recurso do processo</span><span class="sxs-lookup"><span data-stu-id="8ee14-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ee14-105">Contém informações com informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="8ee14-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8ee14-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ee14-106">Properties</span></span>

| <span data-ttu-id="8ee14-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ee14-107">Property</span></span>   | <span data-ttu-id="8ee14-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ee14-108">Type</span></span>|<span data-ttu-id="8ee14-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ee14-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee14-110">accountName</span><span class="sxs-lookup"><span data-stu-id="8ee14-110">accountName</span></span>|<span data-ttu-id="8ee14-111">String</span><span class="sxs-lookup"><span data-stu-id="8ee14-111">String</span></span>|<span data-ttu-id="8ee14-112">Identificador (o contexto de conta do usuário o processo eram executado em) de conta de usuário de exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="8ee14-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="8ee14-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="8ee14-113">commandLine</span></span>|<span data-ttu-id="8ee14-114">String</span><span class="sxs-lookup"><span data-stu-id="8ee14-114">String</span></span>|<span data-ttu-id="8ee14-115">A commandline de invocação do processo completo incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8ee14-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="8ee14-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee14-116">createdDateTime</span></span>|<span data-ttu-id="8ee14-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee14-117">DateTimeOffset</span></span>|<span data-ttu-id="8ee14-118">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="8ee14-118">Time at which the process was started.</span></span> <span data-ttu-id="8ee14-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8ee14-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ee14-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8ee14-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8ee14-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="8ee14-121">fileHash</span></span>|[<span data-ttu-id="8ee14-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="8ee14-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="8ee14-123">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="8ee14-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="8ee14-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="8ee14-124">integrityLevel</span></span>|<span data-ttu-id="8ee14-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="8ee14-125">processIntegrityLevel</span></span>|<span data-ttu-id="8ee14-126">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="8ee14-126">The integrity level of the process.</span></span> <span data-ttu-id="8ee14-127">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="8ee14-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="8ee14-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="8ee14-128">isElevated</span></span>|<span data-ttu-id="8ee14-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="8ee14-129">Boolean</span></span>|<span data-ttu-id="8ee14-130">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="8ee14-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="8ee14-131">name</span><span class="sxs-lookup"><span data-stu-id="8ee14-131">name</span></span>|<span data-ttu-id="8ee14-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ee14-132">String</span></span>|<span data-ttu-id="8ee14-133">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="8ee14-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="8ee14-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee14-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="8ee14-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee14-135">DateTimeOffset</span></span>|<span data-ttu-id="8ee14-136">Data e hora em que o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="8ee14-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="8ee14-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8ee14-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ee14-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8ee14-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8ee14-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="8ee14-139">parentProcessId</span></span>|<span data-ttu-id="8ee14-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8ee14-140">Int32</span></span>|<span data-ttu-id="8ee14-141">O processo de identificação do processo pai.</span><span class="sxs-lookup"><span data-stu-id="8ee14-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="8ee14-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="8ee14-142">parentProcessName</span></span>|<span data-ttu-id="8ee14-143">String</span><span class="sxs-lookup"><span data-stu-id="8ee14-143">String</span></span>|<span data-ttu-id="8ee14-144">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="8ee14-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="8ee14-145">caminho</span><span class="sxs-lookup"><span data-stu-id="8ee14-145">path</span></span>|<span data-ttu-id="8ee14-146">String</span><span class="sxs-lookup"><span data-stu-id="8ee14-146">String</span></span>|<span data-ttu-id="8ee14-147">Caminho completo, incluindo nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8ee14-147">Full path, including filename.</span></span>|
|<span data-ttu-id="8ee14-148">ProcessID</span><span class="sxs-lookup"><span data-stu-id="8ee14-148">processId</span></span>|<span data-ttu-id="8ee14-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8ee14-149">Int32</span></span>|<span data-ttu-id="8ee14-150">O processo de identificação do processo.</span><span class="sxs-lookup"><span data-stu-id="8ee14-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ee14-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ee14-151">JSON representation</span></span>

<span data-ttu-id="8ee14-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ee14-152">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
