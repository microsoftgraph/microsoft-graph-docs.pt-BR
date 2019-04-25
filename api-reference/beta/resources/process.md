---
title: tipo de recurso Process
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563260"
---
# <a name="process-resource-type"></a><span data-ttu-id="eeb13-104">tipo de recurso Process</span><span class="sxs-lookup"><span data-stu-id="eeb13-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeb13-105">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="eeb13-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="eeb13-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeb13-106">Properties</span></span>

| <span data-ttu-id="eeb13-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb13-107">Property</span></span>   | <span data-ttu-id="eeb13-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb13-108">Type</span></span>|<span data-ttu-id="eeb13-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb13-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb13-110">accountName</span><span class="sxs-lookup"><span data-stu-id="eeb13-110">accountName</span></span>|<span data-ttu-id="eeb13-111">String</span><span class="sxs-lookup"><span data-stu-id="eeb13-111">String</span></span>|<span data-ttu-id="eeb13-112">Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="eeb13-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="eeb13-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="eeb13-113">commandLine</span></span>|<span data-ttu-id="eeb13-114">String</span><span class="sxs-lookup"><span data-stu-id="eeb13-114">String</span></span>|<span data-ttu-id="eeb13-115">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="eeb13-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="eeb13-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eeb13-116">createdDateTime</span></span>|<span data-ttu-id="eeb13-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb13-117">DateTimeOffset</span></span>|<span data-ttu-id="eeb13-118">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="eeb13-118">Time at which the process was started.</span></span> <span data-ttu-id="eeb13-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eeb13-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eeb13-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eeb13-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="eeb13-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="eeb13-121">fileHash</span></span>|[<span data-ttu-id="eeb13-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="eeb13-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="eeb13-123">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="eeb13-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="eeb13-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="eeb13-124">integrityLevel</span></span>|<span data-ttu-id="eeb13-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="eeb13-125">processIntegrityLevel</span></span>|<span data-ttu-id="eeb13-126">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="eeb13-126">The integrity level of the process.</span></span> <span data-ttu-id="eeb13-127">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="eeb13-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="eeb13-128">isElevados</span><span class="sxs-lookup"><span data-stu-id="eeb13-128">isElevated</span></span>|<span data-ttu-id="eeb13-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="eeb13-129">Boolean</span></span>|<span data-ttu-id="eeb13-130">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="eeb13-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="eeb13-131">name</span><span class="sxs-lookup"><span data-stu-id="eeb13-131">name</span></span>|<span data-ttu-id="eeb13-132">String</span><span class="sxs-lookup"><span data-stu-id="eeb13-132">String</span></span>|<span data-ttu-id="eeb13-133">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="eeb13-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="eeb13-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeb13-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="eeb13-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb13-135">DateTimeOffset</span></span>|<span data-ttu-id="eeb13-136">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="eeb13-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="eeb13-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eeb13-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eeb13-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eeb13-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="eeb13-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="eeb13-139">parentProcessId</span></span>|<span data-ttu-id="eeb13-140">Int32</span><span class="sxs-lookup"><span data-stu-id="eeb13-140">Int32</span></span>|<span data-ttu-id="eeb13-141">A ID de processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="eeb13-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="eeb13-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="eeb13-142">parentProcessName</span></span>|<span data-ttu-id="eeb13-143">String</span><span class="sxs-lookup"><span data-stu-id="eeb13-143">String</span></span>|<span data-ttu-id="eeb13-144">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="eeb13-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="eeb13-145">caminho</span><span class="sxs-lookup"><span data-stu-id="eeb13-145">path</span></span>|<span data-ttu-id="eeb13-146">String</span><span class="sxs-lookup"><span data-stu-id="eeb13-146">String</span></span>|<span data-ttu-id="eeb13-147">Caminho completo, incluindo o nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="eeb13-147">Full path, including filename.</span></span>|
|<span data-ttu-id="eeb13-148">Identificação</span><span class="sxs-lookup"><span data-stu-id="eeb13-148">processId</span></span>|<span data-ttu-id="eeb13-149">Int32</span><span class="sxs-lookup"><span data-stu-id="eeb13-149">Int32</span></span>|<span data-ttu-id="eeb13-150">A identificação do processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="eeb13-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eeb13-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeb13-151">JSON representation</span></span>

<span data-ttu-id="eeb13-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eeb13-152">The following is a JSON representation of the resource.</span></span>

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
