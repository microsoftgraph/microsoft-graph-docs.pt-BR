# <a name="list-channels"></a><span data-ttu-id="da5c7-101">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="da5c7-101">List channels</span></span>



<span data-ttu-id="da5c7-102">Recupere a lista de [canais](../resources/channel.md) nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="da5c7-102">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="da5c7-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="da5c7-103">Permissions</span></span>
<span data-ttu-id="da5c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da5c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="da5c7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da5c7-106">Permission type</span></span>      | <span data-ttu-id="da5c7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da5c7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da5c7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da5c7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="da5c7-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da5c7-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="da5c7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da5c7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da5c7-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da5c7-111">Not supported.</span></span>    |
|<span data-ttu-id="da5c7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da5c7-112">Application</span></span> | <span data-ttu-id="da5c7-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da5c7-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="da5c7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da5c7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da5c7-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da5c7-115">Optional query parameters</span></span>
<span data-ttu-id="da5c7-116">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da5c7-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da5c7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da5c7-117">Request headers</span></span>
| <span data-ttu-id="da5c7-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da5c7-118">Header</span></span>       | <span data-ttu-id="da5c7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="da5c7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da5c7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="da5c7-120">Authorization</span></span>  | <span data-ttu-id="da5c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da5c7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da5c7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da5c7-123">Request body</span></span>
<span data-ttu-id="da5c7-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da5c7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da5c7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="da5c7-125">Response</span></span>

<span data-ttu-id="da5c7-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da5c7-126">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da5c7-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da5c7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da5c7-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da5c7-128">Request</span></span>
<span data-ttu-id="da5c7-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da5c7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="da5c7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="da5c7-130">Response</span></span>
<span data-ttu-id="da5c7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da5c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
