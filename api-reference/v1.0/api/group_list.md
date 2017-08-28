# <a name="list-groups"></a><span data-ttu-id="df305-101">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="df305-101">List groups</span></span>

<span data-ttu-id="df305-p101">Lista todos os grupos disponíveis em uma organização, incluindo, mas não limitando-se a, grupos do Office 365. As [propriedades padrão](../api/group_get.md#default-properties) de cada grupo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="df305-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="df305-104">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="df305-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="df305-105">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="df305-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="permissions"></a><span data-ttu-id="df305-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df305-106">Permissions</span></span>
<span data-ttu-id="df305-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="df305-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="df305-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df305-109">Permission type</span></span>      | <span data-ttu-id="df305-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df305-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="df305-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df305-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df305-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df305-112">Group.Read.All, Group.Readwrite.All</span></span>    | 
|<span data-ttu-id="df305-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df305-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df305-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df305-114">Not supported.</span></span>    | 
|<span data-ttu-id="df305-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df305-115">Application</span></span> | <span data-ttu-id="df305-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df305-116">Group.Read.All, Group.Readwrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df305-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df305-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="df305-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df305-118">Optional query parameters</span></span>
<span data-ttu-id="df305-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df305-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="df305-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df305-120">Request headers</span></span>
| <span data-ttu-id="df305-121">Nome</span><span class="sxs-lookup"><span data-stu-id="df305-121">Name</span></span>       | <span data-ttu-id="df305-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="df305-122">Type</span></span> | <span data-ttu-id="df305-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="df305-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="df305-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="df305-124">Authorization</span></span>  | <span data-ttu-id="df305-125">string</span><span class="sxs-lookup"><span data-stu-id="df305-125">string</span></span>  | <span data-ttu-id="df305-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df305-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df305-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df305-128">Request body</span></span>
<span data-ttu-id="df305-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df305-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df305-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="df305-130">Response</span></span>

<span data-ttu-id="df305-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df305-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df305-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df305-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df305-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df305-133">Request</span></span>
<span data-ttu-id="df305-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df305-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a><span data-ttu-id="df305-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="df305-135">Response</span></span>
<span data-ttu-id="df305-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df305-136">Here is an example of the response.</span></span>

<span data-ttu-id="df305-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. As [propriedades padrão](../api/group_get.md#default-properties) serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df305-p104">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
