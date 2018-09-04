# <a name="historyitem-resource-type"></a><span data-ttu-id="3baac-101">Tipo de recurso historyItem</span><span class="sxs-lookup"><span data-stu-id="3baac-101">historyItem resource type</span></span>

<span data-ttu-id="3baac-102">Representa um item de histórico de uma [atividade](projectrome_activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3baac-102">Represents a history item for an [activity](projectrome_activity.md) in an app.</span></span> <span data-ttu-id="3baac-103">As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="3baac-103">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="3baac-104">Quando um usuário se compromete com a atividade, o compromisso é capturado como um item do histórico que indica a hora de início e término para a atividade.</span><span class="sxs-lookup"><span data-stu-id="3baac-104">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="3baac-105">À medida que o usuário se compromete novamente com essa atividade ao longo do tempo, vários itens do histórico são registrados para cada atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="3baac-105">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="3baac-106">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **activity** para refletir o período de compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="3baac-106">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="3baac-107">Cada vez que um usuário se compromete novamente com uma atividade, um novo **historyItem** é adicionado à atividade para acumular compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="3baac-107">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="3baac-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3baac-108">Methods</span></span>

|<span data-ttu-id="3baac-109">Método</span><span class="sxs-lookup"><span data-stu-id="3baac-109">Method</span></span> | <span data-ttu-id="3baac-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3baac-110">Return Type</span></span> | <span data-ttu-id="3baac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3baac-111">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="3baac-112">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="3baac-112">Create or replace historyItem</span></span>](../api/projectrome_put_historyitem.md) | <span data-ttu-id="3baac-113">[historyItem](projectrome_historyitem.md)</span><span class="sxs-lookup"><span data-stu-id="3baac-113">Added [historyItem](projectrome_historyitem.md)</span></span> | <span data-ttu-id="3baac-114">Cria ou substitui um **historyItem** existente para a atividade (upsert).</span><span class="sxs-lookup"><span data-stu-id="3baac-114">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="3baac-115">A ID deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="3baac-115">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="3baac-116">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="3baac-116">Delete a historyItem</span></span>](../api/projectrome_delete_historyitem.md) | <span data-ttu-id="3baac-117">Nenhum conteúdo</span><span class="sxs-lookup"><span data-stu-id="3baac-117">204 No Content</span></span> | <span data-ttu-id="3baac-118">Exclui o **historyItem** especificado para a atividade.</span><span class="sxs-lookup"><span data-stu-id="3baac-118">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="3baac-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3baac-119">Properties</span></span>

|<span data-ttu-id="3baac-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3baac-120">Name</span></span> | <span data-ttu-id="3baac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3baac-121">Type</span></span> | <span data-ttu-id="3baac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3baac-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3baac-123">status</span><span class="sxs-lookup"><span data-stu-id="3baac-123">status</span></span> | <span data-ttu-id="3baac-124">status</span><span class="sxs-lookup"><span data-stu-id="3baac-124">status</span></span> | <span data-ttu-id="3baac-125">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="3baac-125">Set by the server.</span></span> <span data-ttu-id="3baac-126">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="3baac-126">A status code used to identify valid objects.</span></span> <span data-ttu-id="3baac-127">Valores: ativo, atualizado, excluído, ignorado.</span><span class="sxs-lookup"><span data-stu-id="3baac-127">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="3baac-128">userTimezone</span><span class="sxs-lookup"><span data-stu-id="3baac-128">userTimezone</span></span> | <span data-ttu-id="3baac-129">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3baac-129">String</span></span> | <span data-ttu-id="3baac-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3baac-130">Optional.</span></span> <span data-ttu-id="3baac-131">O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade.</span><span class="sxs-lookup"><span data-stu-id="3baac-131">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="3baac-132">Valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="3baac-132">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="3baac-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3baac-133">createdDateTime</span></span> | <span data-ttu-id="3baac-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3baac-134">DateTimeOffset</span></span> | <span data-ttu-id="3baac-135">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="3baac-135">Set by the server.</span></span> <span data-ttu-id="3baac-136">DateTime em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="3baac-136">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="3baac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3baac-137">lastModifiedDateTime</span></span> | <span data-ttu-id="3baac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3baac-138">DateTimeOffset</span></span> | <span data-ttu-id="3baac-139">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="3baac-139">Set by the server.</span></span> <span data-ttu-id="3baac-140">DateTime em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="3baac-140">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="3baac-141">id</span><span class="sxs-lookup"><span data-stu-id="3baac-141">id</span></span> | <span data-ttu-id="3baac-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3baac-142">String</span></span> | <span data-ttu-id="3baac-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3baac-143">Required.</span></span> <span data-ttu-id="3baac-144">GUID do conjunto de cliente para o objeto **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="3baac-144">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="3baac-145">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="3baac-145">startedDateTime</span></span> | <span data-ttu-id="3baac-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3baac-146">DateTimeOffset</span></span> | <span data-ttu-id="3baac-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3baac-147">Required.</span></span> <span data-ttu-id="3baac-148">DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="3baac-148">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="3baac-149">Obrigatório para o histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="3baac-149">Required for timeline history.</span></span>|
|<span data-ttu-id="3baac-150">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="3baac-150">lastActiveDateTime</span></span> | <span data-ttu-id="3baac-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3baac-151">DateTimeOffset</span></span> | <span data-ttu-id="3baac-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3baac-152">Optional.</span></span> <span data-ttu-id="3baac-153">DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido como status ativo ou concluído - se for nulo, o status do **historyItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="3baac-153">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="3baac-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3baac-154">expirationDateTime</span></span> | <span data-ttu-id="3baac-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3baac-155">DateTimeOffset</span></span> | <span data-ttu-id="3baac-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3baac-156">Optional.</span></span> <span data-ttu-id="3baac-157">DateTime UTC quando o **historyItem** passará por exclusão irreversível.</span><span class="sxs-lookup"><span data-stu-id="3baac-157">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="3baac-158">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3baac-158">Can be set by the client.</span></span>|
|<span data-ttu-id="3baac-159">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="3baac-159">activeDurationSeconds</span></span> | <span data-ttu-id="3baac-160">int</span><span class="sxs-lookup"><span data-stu-id="3baac-160">int</span></span> | <span data-ttu-id="3baac-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3baac-161">Optional.</span></span> <span data-ttu-id="3baac-162">A duração de participação de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3baac-162">The duration of active user engagement.</span></span> <span data-ttu-id="3baac-163">se não fornecido, isso é calculado do **startedDateTime** e **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3baac-163">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3baac-164">Relações</span><span class="sxs-lookup"><span data-stu-id="3baac-164">Relationships</span></span>

|<span data-ttu-id="3baac-165">Relação</span><span class="sxs-lookup"><span data-stu-id="3baac-165">Relationship</span></span> | <span data-ttu-id="3baac-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="3baac-166">Type</span></span> | <span data-ttu-id="3baac-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="3baac-167">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="3baac-168">atividade</span><span class="sxs-lookup"><span data-stu-id="3baac-168">activity</span></span>| [<span data-ttu-id="3baac-169">userActivity</span><span class="sxs-lookup"><span data-stu-id="3baac-169">userActivity</span></span>](../resources/projectrome_activity.md) | <span data-ttu-id="3baac-170">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3baac-170">Optional.</span></span> <span data-ttu-id="3baac-171">NavigationProperty/Containment; propriedade de navegação à atividade associada.</span><span class="sxs-lookup"><span data-stu-id="3baac-171">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3baac-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3baac-172">JSON representation</span></span>

<span data-ttu-id="3baac-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3baac-173">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
