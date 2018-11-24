# <a name="get-tab"></a><span data-ttu-id="1a87d-101">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="1a87d-101">Get tab</span></span>



<span data-ttu-id="1a87d-102">Recupere as propriedades e relacionamentos da [guia](../resources/teamstab.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1a87d-102">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1a87d-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="1a87d-103">Permissions</span></span>
<span data-ttu-id="1a87d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a87d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a87d-106">Permission type</span></span>      | <span data-ttu-id="1a87d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a87d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a87d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a87d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1a87d-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a87d-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a87d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a87d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a87d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a87d-111">Not supported.</span></span>    |
|<span data-ttu-id="1a87d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a87d-112">Application</span></span> | <span data-ttu-id="1a87d-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a87d-113">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1a87d-114">Atualmente, somente [permissões delegadas](../../../concepts/permissions_reference.md) têm suporte para esta operação.</span><span class="sxs-lookup"><span data-stu-id="1a87d-114">Currently, only [delegated permissions](../../../concepts/permissions_reference.md) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a87d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a87d-115">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a87d-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a87d-116">Optional query parameters</span></span>

<span data-ttu-id="1a87d-117">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a87d-117">This method supports the $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a87d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a87d-118">Request headers</span></span>
| <span data-ttu-id="1a87d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a87d-119">Header</span></span>       | <span data-ttu-id="1a87d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1a87d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a87d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a87d-121">Authorization</span></span>  | <span data-ttu-id="1a87d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a87d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a87d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a87d-124">Request body</span></span>
<span data-ttu-id="1a87d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a87d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a87d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a87d-126">Response</span></span>

<span data-ttu-id="1a87d-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a87d-127">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a87d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a87d-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1a87d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a87d-129">Request</span></span>
<span data-ttu-id="1a87d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a87d-130">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="1a87d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a87d-131">Response</span></span>
<span data-ttu-id="1a87d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a87d-132">The following is an example of the response.</span></span> 

><span data-ttu-id="1a87d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a87d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
