# <a name="create-channel"></a><span data-ttu-id="98154-101">Criar canal</span><span class="sxs-lookup"><span data-stu-id="98154-101">Create Channel</span></span>



<span data-ttu-id="98154-102">Crie um novo [canal](../resources/channel.md) em um Microsoft Team, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98154-102">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="98154-103">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="98154-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="98154-104">Para obter detalhes, consulte a [lista de problemas conhecidos do](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="98154-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="98154-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="98154-105">Permissions</span></span>
<span data-ttu-id="98154-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98154-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="98154-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98154-108">Permission type</span></span>      | <span data-ttu-id="98154-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98154-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98154-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98154-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98154-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98154-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98154-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98154-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98154-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98154-113">Not supported.</span></span>    |
|<span data-ttu-id="98154-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98154-114">Application</span></span> | <span data-ttu-id="98154-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98154-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="98154-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98154-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="98154-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98154-117">Request headers</span></span>
| <span data-ttu-id="98154-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98154-118">Header</span></span>       | <span data-ttu-id="98154-119">Valor</span><span class="sxs-lookup"><span data-stu-id="98154-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98154-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="98154-120">Authorization</span></span>  | <span data-ttu-id="98154-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98154-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98154-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98154-123">Content-Type</span></span>  | <span data-ttu-id="98154-124">application/json</span><span class="sxs-lookup"><span data-stu-id="98154-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98154-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98154-125">Request body</span></span>
<span data-ttu-id="98154-126">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="98154-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98154-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="98154-127">Response</span></span>

<span data-ttu-id="98154-128">Se tiver êxito, este método retornará `201 Created` objeto de código e o [canal](../resources/channel.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98154-128">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98154-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98154-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98154-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98154-130">Request</span></span>
<span data-ttu-id="98154-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98154-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="98154-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="98154-132">Response</span></span>
<span data-ttu-id="98154-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98154-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
