# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="baab6-101">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="baab6-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="baab6-p101">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="baab6-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="baab6-105">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="baab6-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="baab6-106">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](directoryobject_getmemberobjects.md) ou [getMemberGroups](directoryobject_getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="baab6-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="baab6-107">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="baab6-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="baab6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="baab6-108">Permissions</span></span>

<span data-ttu-id="baab6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="baab6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="baab6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baab6-111">Permission type</span></span>      | <span data-ttu-id="baab6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="baab6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baab6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baab6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="baab6-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="baab6-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="baab6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baab6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baab6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baab6-116">Not supported.</span></span>    |
|<span data-ttu-id="baab6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baab6-117">Application</span></span> | <span data-ttu-id="baab6-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="baab6-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baab6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baab6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="baab6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baab6-120">Request headers</span></span>

| <span data-ttu-id="baab6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="baab6-121">Name</span></span>       | <span data-ttu-id="baab6-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="baab6-122">Type</span></span> | <span data-ttu-id="baab6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="baab6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="baab6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="baab6-124">Authorization</span></span>  | <span data-ttu-id="baab6-125">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="baab6-125">string</span></span>  | <span data-ttu-id="baab6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baab6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="baab6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="baab6-128">Content-Type</span></span>  | <span data-ttu-id="baab6-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="baab6-129">string</span></span> | <span data-ttu-id="baab6-130">application/json</span><span class="sxs-lookup"><span data-stu-id="baab6-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="baab6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baab6-131">Request body</span></span>

<span data-ttu-id="baab6-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baab6-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="baab6-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="baab6-133">Parameter</span></span>   | <span data-ttu-id="baab6-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="baab6-134">Type</span></span> |<span data-ttu-id="baab6-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="baab6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baab6-136">ids</span><span class="sxs-lookup"><span data-stu-id="baab6-136">ids</span></span>|<span data-ttu-id="baab6-137">Conjunto de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="baab6-137">String collection</span></span>| <span data-ttu-id="baab6-p104">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="baab6-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="baab6-140">tipos</span><span class="sxs-lookup"><span data-stu-id="baab6-140">types</span></span>|<span data-ttu-id="baab6-141">Conjunto de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="baab6-141">String collection</span></span>| <span data-ttu-id="baab6-142">Uma coleção dos tipos de recursos que especifica o conjunto de coleções de recursos a pesquisar.</span><span class="sxs-lookup"><span data-stu-id="baab6-142">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="baab6-143">Se não especificado, o padrão é [directoryObject](../resources/directoryobject.md), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="baab6-143">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="baab6-144">Qualquer objeto que derive de `directoryObject` pode ser especificado na coleção; por exemplo: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md)e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="baab6-144">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="baab6-145">Os valores não diferenciam entre maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="baab6-145">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="baab6-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="baab6-146">Response</span></span>

<span data-ttu-id="baab6-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baab6-147">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baab6-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baab6-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="baab6-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baab6-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="baab6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="baab6-150">Response</span></span>

<span data-ttu-id="baab6-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baab6-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
