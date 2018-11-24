# <a name="delete-channel"></a><span data-ttu-id="568d6-101">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="568d6-101">Delete channel</span></span>



<span data-ttu-id="568d6-102">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="568d6-102">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="568d6-103">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="568d6-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="568d6-104">Para obter detalhes, consulte a [lista de problemas conhecidos do](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="568d6-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

> <span data-ttu-id="568d6-105">**Observação**: os dados no canais excluídos continuarão a serem armazenados durante várias semanas permitir que o proprietário de equipe para o canal de recuperação excluído.</span><span class="sxs-lookup"><span data-stu-id="568d6-105">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="568d6-106">Durante esse tempo, um novo canal com o mesmo displayName não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="568d6-106">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="568d6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="568d6-107">Permissions</span></span>
<span data-ttu-id="568d6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="568d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="568d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="568d6-110">Permission type</span></span>      | <span data-ttu-id="568d6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="568d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="568d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="568d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="568d6-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d6-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="568d6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="568d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="568d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="568d6-115">Not supported.</span></span>    |
|<span data-ttu-id="568d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="568d6-116">Application</span></span> | <span data-ttu-id="568d6-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d6-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="568d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="568d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="568d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="568d6-119">Request headers</span></span>
| <span data-ttu-id="568d6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="568d6-120">Header</span></span>       | <span data-ttu-id="568d6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="568d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="568d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="568d6-122">Authorization</span></span>  | <span data-ttu-id="568d6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="568d6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="568d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="568d6-125">Request body</span></span>
<span data-ttu-id="568d6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="568d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="568d6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="568d6-127">Response</span></span>

<span data-ttu-id="568d6-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="568d6-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="568d6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="568d6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="568d6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="568d6-131">Request</span></span>
<span data-ttu-id="568d6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="568d6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="568d6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="568d6-133">Response</span></span>

<span data-ttu-id="568d6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="568d6-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
