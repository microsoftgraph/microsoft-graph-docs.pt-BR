# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="fc359-101">tipo de recurso de dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc359-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="fc359-102">Representa uma operação de diretiva de dados enviados.</span><span class="sxs-lookup"><span data-stu-id="fc359-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="fc359-103">Ele contém as informações necessárias para rastrear o status de uma operação.</span><span class="sxs-lookup"><span data-stu-id="fc359-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="fc359-104">Por exemplo, um administrador da empresa pode enviar uma solicitação de operação de política de dados para exportar os dados da empresa de um funcionário e, em seguida, rastrear mais tarde que a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc359-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="fc359-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc359-105">Methods</span></span>

| <span data-ttu-id="fc359-106">Método</span><span class="sxs-lookup"><span data-stu-id="fc359-106">Method</span></span>           | <span data-ttu-id="fc359-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc359-107">Return Type</span></span>    |<span data-ttu-id="fc359-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc359-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc359-109">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc359-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="fc359-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc359-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="fc359-111">Recupere as propriedades do objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="fc359-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="fc359-112">Exportar dados pessoais</span><span class="sxs-lookup"><span data-stu-id="fc359-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="fc359-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc359-113">None</span></span> |<span data-ttu-id="fc359-114">Enviar uma solicitação de operação de política de dados para exportar os dados do usuário organizacionais que posteriormente podem ser lidos com [obter dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="fc359-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="fc359-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc359-115">Properties</span></span>

> <span data-ttu-id="fc359-116">**Observação:** Todas as propriedades desse recurso são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc359-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="fc359-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc359-117">Property</span></span>     | <span data-ttu-id="fc359-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc359-118">Type</span></span>   |<span data-ttu-id="fc359-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc359-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc359-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc359-120">completedDateTime</span></span>|<span data-ttu-id="fc359-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc359-121">DateTimeOffset</span></span>|<span data-ttu-id="fc359-122">Representa quando a solicitação para esta operação de política de dados foi concluída, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fc359-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fc359-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fc359-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fc359-124">Nulo até que a operação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="fc359-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="fc359-125">id</span><span class="sxs-lookup"><span data-stu-id="fc359-125">id</span></span>|<span data-ttu-id="fc359-126">String</span><span class="sxs-lookup"><span data-stu-id="fc359-126">String</span></span>| <span data-ttu-id="fc359-127">Chave exclusiva para essa operação.</span><span class="sxs-lookup"><span data-stu-id="fc359-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="fc359-128">status</span><span class="sxs-lookup"><span data-stu-id="fc359-128">status</span></span>|<span data-ttu-id="fc359-129">string</span><span class="sxs-lookup"><span data-stu-id="fc359-129">string</span></span>| <span data-ttu-id="fc359-130">Os valores possíveis são: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fc359-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fc359-131">storageLocation</span><span class="sxs-lookup"><span data-stu-id="fc359-131">storageLocation</span></span>|<span data-ttu-id="fc359-132">String</span><span class="sxs-lookup"><span data-stu-id="fc359-132">String</span></span>|<span data-ttu-id="fc359-133">O local da URL para onde os dados está sendo exportados para solicitações de exportação.</span><span class="sxs-lookup"><span data-stu-id="fc359-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="fc359-134">userId</span><span class="sxs-lookup"><span data-stu-id="fc359-134">userId</span></span>|<span data-ttu-id="fc359-135">String</span><span class="sxs-lookup"><span data-stu-id="fc359-135">String</span></span>|<span data-ttu-id="fc359-136">A identificação do usuário no qual a operação é executada.</span><span class="sxs-lookup"><span data-stu-id="fc359-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="fc359-137">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc359-137">submittedDateTime</span></span>|<span data-ttu-id="fc359-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc359-138">DateTimeOffset</span></span>|<span data-ttu-id="fc359-139">Representa quando a solicitação para esta operação de dados foi enviada, em tempo de UTC, usando o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fc359-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fc359-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fc359-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc359-141">progresso</span><span class="sxs-lookup"><span data-stu-id="fc359-141">progress</span></span>|<span data-ttu-id="fc359-142">String</span><span class="sxs-lookup"><span data-stu-id="fc359-142">String</span></span>|<span data-ttu-id="fc359-143">Especifica o progresso de uma operação.</span><span class="sxs-lookup"><span data-stu-id="fc359-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc359-144">Relações</span><span class="sxs-lookup"><span data-stu-id="fc359-144">Relationships</span></span>
<span data-ttu-id="fc359-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc359-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fc359-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc359-146">JSON representation</span></span>

<span data-ttu-id="fc359-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc359-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
