# <a name="get-channel"></a><span data-ttu-id="e9c3c-101">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="e9c3c-101">Get channel</span></span>



<span data-ttu-id="e9c3c-102">Recupere as propriedades e relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e9c3c-102">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9c3c-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="e9c3c-103">Permissions</span></span>
<span data-ttu-id="e9c3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9c3c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9c3c-106">Permission type</span></span>      | <span data-ttu-id="e9c3c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9c3c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9c3c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9c3c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e9c3c-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9c3c-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9c3c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9c3c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9c3c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-111">Not supported.</span></span>    |
|<span data-ttu-id="e9c3c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9c3c-112">Application</span></span> | <span data-ttu-id="e9c3c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9c3c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="e9c3c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9c3c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9c3c-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9c3c-115">Optional query parameters</span></span>

<span data-ttu-id="e9c3c-116">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9c3c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c3c-117">Request headers</span></span>
| <span data-ttu-id="e9c3c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9c3c-118">Header</span></span>       | <span data-ttu-id="e9c3c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e9c3c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9c3c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9c3c-120">Authorization</span></span>  | <span data-ttu-id="e9c3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9c3c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c3c-123">Request body</span></span>
<span data-ttu-id="e9c3c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9c3c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9c3c-125">Response</span></span>

<span data-ttu-id="e9c3c-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-126">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9c3c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9c3c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9c3c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c3c-128">Request</span></span>
<span data-ttu-id="e9c3c-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="e9c3c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9c3c-130">Response</span></span>
<span data-ttu-id="e9c3c-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-131">Here is an example of the response.</span></span> 

><span data-ttu-id="e9c3c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9c3c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
