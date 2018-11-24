# <a name="update-team"></a><span data-ttu-id="64348-101">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="64348-101">Update team</span></span>



<span data-ttu-id="64348-102">Atualize as propriedades da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="64348-102">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64348-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="64348-103">Permissions</span></span>
<span data-ttu-id="64348-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="64348-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64348-106">Permission type</span></span>      | <span data-ttu-id="64348-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64348-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64348-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64348-108">Delegated (work or school account)</span></span> | <span data-ttu-id="64348-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64348-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64348-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64348-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64348-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64348-111">Not supported.</span></span>    |
|<span data-ttu-id="64348-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64348-112">Application</span></span> | <span data-ttu-id="64348-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64348-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="64348-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64348-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="64348-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64348-115">Request headers</span></span>
| <span data-ttu-id="64348-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64348-116">Header</span></span>       | <span data-ttu-id="64348-117">Valor</span><span class="sxs-lookup"><span data-stu-id="64348-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64348-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="64348-118">Authorization</span></span>  | <span data-ttu-id="64348-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64348-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64348-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64348-121">Content-Type</span></span>  | <span data-ttu-id="64348-122">application/json</span><span class="sxs-lookup"><span data-stu-id="64348-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64348-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64348-123">Request body</span></span>
<span data-ttu-id="64348-124">No corpo da solicitação, fornece uma representação JSON do objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="64348-124">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64348-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="64348-125">Response</span></span>

<span data-ttu-id="64348-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64348-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64348-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64348-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="64348-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64348-128">Request</span></span>
<span data-ttu-id="64348-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64348-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="64348-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="64348-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
