# <a name="process-resource-type"></a><span data-ttu-id="292a0-101">tipo de recurso processo</span><span class="sxs-lookup"><span data-stu-id="292a0-101">process resource type</span></span>

<span data-ttu-id="292a0-102">Contém informações com estado sobre o processo relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="292a0-102">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="292a0-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="292a0-103">Properties</span></span>

| <span data-ttu-id="292a0-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="292a0-104">Property</span></span>   | <span data-ttu-id="292a0-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="292a0-105">Type</span></span>|<span data-ttu-id="292a0-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="292a0-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="292a0-107">accountName</span><span class="sxs-lookup"><span data-stu-id="292a0-107">accountName</span></span>|<span data-ttu-id="292a0-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="292a0-108">String</span></span>|<span data-ttu-id="292a0-109">Identificador da conta do usuário (o contexto de conta do usuário no qual o processo foi executado) por exemplo, AccountName, SID, entre outros.</span><span class="sxs-lookup"><span data-stu-id="292a0-109">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="292a0-110">commandLine</span><span class="sxs-lookup"><span data-stu-id="292a0-110">commandLine</span></span>|<span data-ttu-id="292a0-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="292a0-111">String</span></span>|<span data-ttu-id="292a0-112">A commandline de invocação do processo completo, incluindo todos os parâmetros.</span><span class="sxs-lookup"><span data-stu-id="292a0-112">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="292a0-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="292a0-113">createdDateTime</span></span>|<span data-ttu-id="292a0-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="292a0-114">DateTimeOffset</span></span>|<span data-ttu-id="292a0-115">Hora em que o processo foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="292a0-115">Time at which the process was started.</span></span> <span data-ttu-id="292a0-116">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="292a0-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="292a0-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="292a0-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="292a0-118">fileHash</span><span class="sxs-lookup"><span data-stu-id="292a0-118">fileHash</span></span>|[<span data-ttu-id="292a0-119">fileHash</span><span class="sxs-lookup"><span data-stu-id="292a0-119">fileHash</span></span>](filehash.md)|<span data-ttu-id="292a0-120">Tipo Complex contendo hashes de arquivo (criptográficos e sensíveis à localização).</span><span class="sxs-lookup"><span data-stu-id="292a0-120">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="292a0-121">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="292a0-121">integrityLevel</span></span>|<span data-ttu-id="292a0-122">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="292a0-122">processIntegrityLevel</span></span>|<span data-ttu-id="292a0-123">O nível de integridade do processo.</span><span class="sxs-lookup"><span data-stu-id="292a0-123">The integrity level of the process.</span></span> <span data-ttu-id="292a0-124">Os valores possíveis são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span><span class="sxs-lookup"><span data-stu-id="292a0-124">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="292a0-125">isElevated</span><span class="sxs-lookup"><span data-stu-id="292a0-125">isElevated</span></span>|<span data-ttu-id="292a0-126">Booleano</span><span class="sxs-lookup"><span data-stu-id="292a0-126">Boolean</span></span>|<span data-ttu-id="292a0-127">True se o processo for elevado.</span><span class="sxs-lookup"><span data-stu-id="292a0-127">True if the process is elevated.</span></span>|
|<span data-ttu-id="292a0-128">name</span><span class="sxs-lookup"><span data-stu-id="292a0-128">name</span></span>|<span data-ttu-id="292a0-129">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="292a0-129">String</span></span>|<span data-ttu-id="292a0-130">O nome do arquivo de imagem do processo.</span><span class="sxs-lookup"><span data-stu-id="292a0-130">The name of the process' Image file.</span></span>|
|<span data-ttu-id="292a0-131">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="292a0-131">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="292a0-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="292a0-132">DateTimeOffset</span></span>|<span data-ttu-id="292a0-133">Data e hora em que o processo pai foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="292a0-133">DateTime at which the parent process was started.</span></span> <span data-ttu-id="292a0-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="292a0-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="292a0-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="292a0-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="292a0-136">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="292a0-136">parentProcessId</span></span>|<span data-ttu-id="292a0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="292a0-137">Int32</span></span>|<span data-ttu-id="292a0-138">A ID de Processo (PID) do processo pai.</span><span class="sxs-lookup"><span data-stu-id="292a0-138">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="292a0-139">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="292a0-139">parentProcessName</span></span>|<span data-ttu-id="292a0-140">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="292a0-140">String</span></span>|<span data-ttu-id="292a0-141">O nome do arquivo de imagem do processo pai.</span><span class="sxs-lookup"><span data-stu-id="292a0-141">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="292a0-142">path</span><span class="sxs-lookup"><span data-stu-id="292a0-142">path</span></span>|<span data-ttu-id="292a0-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="292a0-143">String</span></span>|<span data-ttu-id="292a0-144">Caminho completo, incluindo nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="292a0-144">Full path, including filename.</span></span>|
|<span data-ttu-id="292a0-145">processId</span><span class="sxs-lookup"><span data-stu-id="292a0-145">processId</span></span>|<span data-ttu-id="292a0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="292a0-146">Int32</span></span>|<span data-ttu-id="292a0-147">A ID de Processo (PID) do processo.</span><span class="sxs-lookup"><span data-stu-id="292a0-147">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="292a0-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="292a0-148">JSON representation</span></span>

<span data-ttu-id="292a0-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="292a0-149">The following is a JSON representation of the resource.</span></span>

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