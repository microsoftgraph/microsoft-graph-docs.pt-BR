# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="a041e-101">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="a041e-101">List groupLifecyclePolicies</span></span>

<span data-ttu-id="a041e-102">Recupera uma lista de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) à qual um grupo pertence.</span><span class="sxs-lookup"><span data-stu-id="a041e-102">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="a041e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a041e-103">Permissions</span></span>

<span data-ttu-id="a041e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a041e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a041e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a041e-106">Permission type</span></span>      | <span data-ttu-id="a041e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a041e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a041e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a041e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a041e-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a041e-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="a041e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a041e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a041e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a041e-111">Not supported.</span></span>    |
|<span data-ttu-id="a041e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a041e-112">Application</span></span> | <span data-ttu-id="a041e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a041e-113">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a041e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a041e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a041e-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a041e-115">Optional query parameters</span></span>
<span data-ttu-id="a041e-116">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a041e-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a041e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a041e-117">Request headers</span></span>
| <span data-ttu-id="a041e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a041e-118">Name</span></span> | <span data-ttu-id="a041e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a041e-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a041e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a041e-120">Authorization</span></span> | <span data-ttu-id="a041e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a041e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a041e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a041e-123">Request body</span></span>
<span data-ttu-id="a041e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a041e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a041e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a041e-125">Response</span></span>
<span data-ttu-id="a041e-126">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a041e-126">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a041e-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a041e-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a041e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a041e-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="a041e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a041e-129">Response</span></span>

<span data-ttu-id="a041e-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a041e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->