# <a name="group-renew"></a><span data-ttu-id="8853f-101">group: renew</span><span class="sxs-lookup"><span data-stu-id="8853f-101">group: renew</span></span>

<span data-ttu-id="8853f-102">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="8853f-102">Renews a group's expiration.</span></span> <span data-ttu-id="8853f-103">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="8853f-103">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8853f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="8853f-104">Permissions</span></span>

<span data-ttu-id="8853f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8853f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="8853f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8853f-107">Permission type</span></span>      | <span data-ttu-id="8853f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8853f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8853f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8853f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8853f-110">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8853f-110">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8853f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8853f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8853f-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8853f-112">Not supported</span></span> |
|<span data-ttu-id="8853f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8853f-113">Application</span></span> | <span data-ttu-id="8853f-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8853f-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8853f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8853f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a><span data-ttu-id="8853f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8853f-116">Request headers</span></span>
| <span data-ttu-id="8853f-117">Nome</span><span class="sxs-lookup"><span data-stu-id="8853f-117">Name</span></span>       | <span data-ttu-id="8853f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8853f-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8853f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8853f-119">Authorization</span></span>  | <span data-ttu-id="8853f-120">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8853f-120">Bearer %token%</span></span> |


## <a name="request-body"></a><span data-ttu-id="8853f-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8853f-121">Request body</span></span>

<span data-ttu-id="8853f-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8853f-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8853f-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="8853f-123">Response</span></span>

<span data-ttu-id="8853f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8853f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8853f-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8853f-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8853f-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8853f-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a><span data-ttu-id="8853f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8853f-128">Response</span></span>
<span data-ttu-id="8853f-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8853f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->