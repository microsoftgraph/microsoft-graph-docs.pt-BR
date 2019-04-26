---
title: tipo de recurso Process
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 244c809008eaea286f3048ed103d1b5320e0765e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344263"
---
# <a name="process-resource-type"></a><span data-ttu-id="3e5bd-104">tipo de recurso Process</span><span class="sxs-lookup"><span data-stu-id="3e5bd-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e5bd-105">Contém informações de estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="3e5bd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e5bd-106">Properties</span></span>

| <span data-ttu-id="3e5bd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e5bd-107">Property</span></span>   | <span data-ttu-id="3e5bd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e5bd-108">Type</span></span>|<span data-ttu-id="3e5bd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e5bd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e5bd-110">accountName</span><span class="sxs-lookup"><span data-stu-id="3e5bd-110">accountName</span></span>|<span data-ttu-id="3e5bd-111">String</span><span class="sxs-lookup"><span data-stu-id="3e5bd-111">String</span></span>|<span data-ttu-id="3e5bd-112">Identificador da conta de usuário (contexto da conta de usuário o processo executado em) por exemplo, AccountName, SID e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="3e5bd-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="3e5bd-113">commandLine</span></span>|<span data-ttu-id="3e5bd-114">String</span><span class="sxs-lookup"><span data-stu-id="3e5bd-114">String</span></span>|<span data-ttu-id="3e5bd-115">A linha de comando de invocação de processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="3e5bd-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e5bd-116">createdDateTime</span></span>|<span data-ttu-id="3e5bd-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e5bd-117">DateTimeOffset</span></span>|<span data-ttu-id="3e5bd-118">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-118">Time at which the process was started.</span></span> <span data-ttu-id="3e5bd-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e5bd-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3e5bd-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="3e5bd-121">fileHash</span></span>|[<span data-ttu-id="3e5bd-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="3e5bd-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="3e5bd-123">Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).</span><span class="sxs-lookup"><span data-stu-id="3e5bd-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="3e5bd-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="3e5bd-124">integrityLevel</span></span>|<span data-ttu-id="3e5bd-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="3e5bd-125">processIntegrityLevel</span></span>|<span data-ttu-id="3e5bd-126">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-126">The integrity level of the process.</span></span> <span data-ttu-id="3e5bd-127">Os possíveis valores são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="3e5bd-128">isElevados</span><span class="sxs-lookup"><span data-stu-id="3e5bd-128">isElevated</span></span>|<span data-ttu-id="3e5bd-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e5bd-129">Boolean</span></span>|<span data-ttu-id="3e5bd-130">True se o processo é elevado.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="3e5bd-131">name</span><span class="sxs-lookup"><span data-stu-id="3e5bd-131">name</span></span>|<span data-ttu-id="3e5bd-132">String</span><span class="sxs-lookup"><span data-stu-id="3e5bd-132">String</span></span>|<span data-ttu-id="3e5bd-133">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="3e5bd-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e5bd-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="3e5bd-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e5bd-135">DateTimeOffset</span></span>|<span data-ttu-id="3e5bd-136">DateTime no qual o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="3e5bd-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e5bd-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3e5bd-139">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="3e5bd-139">parentProcessId</span></span>|<span data-ttu-id="3e5bd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3e5bd-140">Int32</span></span>|<span data-ttu-id="3e5bd-141">A ID de processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="3e5bd-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="3e5bd-142">parentProcessName</span></span>|<span data-ttu-id="3e5bd-143">String</span><span class="sxs-lookup"><span data-stu-id="3e5bd-143">String</span></span>|<span data-ttu-id="3e5bd-144">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="3e5bd-145">caminho</span><span class="sxs-lookup"><span data-stu-id="3e5bd-145">path</span></span>|<span data-ttu-id="3e5bd-146">String</span><span class="sxs-lookup"><span data-stu-id="3e5bd-146">String</span></span>|<span data-ttu-id="3e5bd-147">Caminho completo, incluindo o nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-147">Full path, including filename.</span></span>|
|<span data-ttu-id="3e5bd-148">Identificação</span><span class="sxs-lookup"><span data-stu-id="3e5bd-148">processId</span></span>|<span data-ttu-id="3e5bd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3e5bd-149">Int32</span></span>|<span data-ttu-id="3e5bd-150">A identificação do processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e5bd-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e5bd-151">JSON representation</span></span>

<span data-ttu-id="3e5bd-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e5bd-152">The following is a JSON representation of the resource.</span></span>

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
