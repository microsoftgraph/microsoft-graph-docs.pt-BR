# <a name="get-team"></a><span data-ttu-id="7f7c5-101">Obtenha a equipe</span><span class="sxs-lookup"><span data-stu-id="7f7c5-101">Get team</span></span>



<span data-ttu-id="7f7c5-102">Recupere as propriedades e relacionamentos da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-102">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f7c5-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f7c5-103">Permissions</span></span>
<span data-ttu-id="7f7c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f7c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f7c5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f7c5-106">Permission type</span></span>      | <span data-ttu-id="7f7c5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f7c5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f7c5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f7c5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7f7c5-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7c5-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f7c5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f7c5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f7c5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-111">Not supported.</span></span>    |
|<span data-ttu-id="7f7c5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f7c5-112">Application</span></span> | <span data-ttu-id="7f7c5-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7c5-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7f7c5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7c5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f7c5-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f7c5-115">Optional query parameters</span></span>
<span data-ttu-id="7f7c5-116">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-116">This method supports the $select and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f7c5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7c5-117">Request headers</span></span>
| <span data-ttu-id="7f7c5-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f7c5-118">Header</span></span>       | <span data-ttu-id="7f7c5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7f7c5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f7c5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f7c5-120">Authorization</span></span>  | <span data-ttu-id="7f7c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f7c5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7c5-123">Request body</span></span>
<span data-ttu-id="7f7c5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f7c5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7c5-125">Response</span></span>

<span data-ttu-id="7f7c5-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-126">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f7c5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f7c5-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f7c5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7c5-128">Request</span></span>
<span data-ttu-id="7f7c5-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="7f7c5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7c5-130">Response</span></span>
<span data-ttu-id="7f7c5-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-131">The following is an example of the response.</span></span> 

><span data-ttu-id="7f7c5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f7c5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
