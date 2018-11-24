# <a name="create-team"></a><span data-ttu-id="d3428-101">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="d3428-101">Create team</span></span>



<span data-ttu-id="d3428-102">Crie uma nova [equipe](../resources/team.md) em um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="d3428-102">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="d3428-103">Para criar uma equipe, o grupo deve ter um mínimo de um proprietário.</span><span class="sxs-lookup"><span data-stu-id="d3428-103">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="d3428-104">Se o grupo foi criado há menos de 15 minutos, é possível para a chamada de equipe criar falha com um código de 404 erro devido aos atrasos de replicação.</span><span class="sxs-lookup"><span data-stu-id="d3428-104">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="d3428-105">O padrão recomendado é repetir a chamada de equipe criar três vezes, com um atraso de segunda 10 entre chamadas.</span><span class="sxs-lookup"><span data-stu-id="d3428-105">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3428-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d3428-106">Permissions</span></span>

<span data-ttu-id="d3428-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3428-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3428-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3428-109">Permission type</span></span>      | <span data-ttu-id="d3428-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3428-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3428-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3428-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3428-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3428-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3428-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3428-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3428-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3428-114">Not supported.</span></span>    |
|<span data-ttu-id="d3428-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3428-115">Application</span></span> | <span data-ttu-id="d3428-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3428-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3428-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3428-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="d3428-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3428-118">Request headers</span></span>

| <span data-ttu-id="d3428-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3428-119">Header</span></span>       | <span data-ttu-id="d3428-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d3428-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3428-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3428-121">Authorization</span></span>  | <span data-ttu-id="d3428-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3428-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3428-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3428-124">Content-Type</span></span>  | <span data-ttu-id="d3428-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3428-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3428-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3428-126">Request body</span></span>

<span data-ttu-id="d3428-127">No corpo da solicitação, fornece uma representação JSON de um objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="d3428-127">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3428-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3428-128">Response</span></span>

<span data-ttu-id="d3428-129">Se tiver êxito, esse método deve retornar uma `201 Created` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3428-129">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3428-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3428-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3428-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3428-131">Request</span></span>

<span data-ttu-id="d3428-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3428-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

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

#### <a name="response"></a><span data-ttu-id="d3428-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3428-133">Response</span></span>

<span data-ttu-id="d3428-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3428-134">The following is an example of the response.</span></span> 

><span data-ttu-id="d3428-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3428-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="d3428-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d3428-137">See also</span></span>

- [<span data-ttu-id="d3428-138">Criando um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="d3428-138">Creating a group with a team</span></span>](../../../concepts/teams-create-group-and-team.md)
