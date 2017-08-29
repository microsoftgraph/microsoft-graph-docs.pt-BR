# <a name="get-entity"></a><span data-ttu-id="7c311-101">Obter entidade</span><span class="sxs-lookup"><span data-stu-id="7c311-101">Get entity</span></span>

<span data-ttu-id="7c311-102">Recupera as propriedades e os relacionamentos do objeto de entidade.</span><span class="sxs-lookup"><span data-stu-id="7c311-102">Retrieve the properties and relationships of entity object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c311-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c311-103">Permissions</span></span>
<span data-ttu-id="7c311-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c311-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c311-106">Permission type</span></span>      | <span data-ttu-id="7c311-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c311-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c311-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c311-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7c311-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c311-109">Not supported.</span></span>    |
|<span data-ttu-id="7c311-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c311-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c311-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c311-111">Not supported.</span></span>    |
|<span data-ttu-id="7c311-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c311-112">Application</span></span> | <span data-ttu-id="7c311-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c311-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c311-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c311-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http

```
## <a name="optional-query-parameters"></a><span data-ttu-id="7c311-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c311-115">Optional query parameters</span></span>
<span data-ttu-id="7c311-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c311-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7c311-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c311-117">Request headers</span></span>
| <span data-ttu-id="7c311-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7c311-118">Name</span></span>       | <span data-ttu-id="7c311-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c311-119">Type</span></span> | <span data-ttu-id="7c311-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c311-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c311-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c311-121">Authorization</span></span>  | <span data-ttu-id="7c311-122">string</span><span class="sxs-lookup"><span data-stu-id="7c311-122">string</span></span>  | <span data-ttu-id="7c311-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c311-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c311-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c311-125">Request body</span></span>
<span data-ttu-id="7c311-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c311-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c311-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c311-127">Response</span></span>

<span data-ttu-id="7c311-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [entity](../resources/entity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c311-128">If successful, this method returns a `200 OK` response code and [entity](../resources/entity.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c311-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c311-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c311-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c311-130">Request</span></span>
<span data-ttu-id="7c311-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c311-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_entity"
}-->
```http

```
##### <a name="response"></a><span data-ttu-id="7c311-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c311-132">Response</span></span>
<span data-ttu-id="7c311-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c311-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
