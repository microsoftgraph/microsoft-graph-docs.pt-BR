# <a name="get-group"></a><span data-ttu-id="4f9af-101">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="4f9af-101">Get group</span></span>
<span data-ttu-id="4f9af-102">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="4f9af-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="4f9af-103">Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="4f9af-103">Default properties</span></span>

<span data-ttu-id="4f9af-p101">O seguinte item representa o conjunto padrão de propriedades que são retornadas ao obter ou listar grupos. Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4f9af-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="4f9af-106">description</span><span class="sxs-lookup"><span data-stu-id="4f9af-106">description</span></span>
* <span data-ttu-id="4f9af-107">displayName</span><span class="sxs-lookup"><span data-stu-id="4f9af-107">displayName</span></span>
* <span data-ttu-id="4f9af-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="4f9af-108">groupTypes</span></span>
* <span data-ttu-id="4f9af-109">id</span><span class="sxs-lookup"><span data-stu-id="4f9af-109">id</span></span>
* <span data-ttu-id="4f9af-110">Email</span><span class="sxs-lookup"><span data-stu-id="4f9af-110">mail</span></span>
* <span data-ttu-id="4f9af-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4f9af-111">mailEnabled</span></span>
* <span data-ttu-id="4f9af-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4f9af-112">mailNickname</span></span>
* <span data-ttu-id="4f9af-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4f9af-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="4f9af-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f9af-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="4f9af-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="4f9af-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="4f9af-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="4f9af-116">proxyAddresses</span></span>
* <span data-ttu-id="4f9af-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4f9af-117">securityEnabled</span></span>
* <span data-ttu-id="4f9af-118">visibilidade</span><span class="sxs-lookup"><span data-stu-id="4f9af-118">visibility</span></span>

<span data-ttu-id="4f9af-119">As seguintes propriedades de grupo não são retornadas por padrão:</span><span class="sxs-lookup"><span data-stu-id="4f9af-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="4f9af-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="4f9af-120">allowExternalSenders</span></span>
* <span data-ttu-id="4f9af-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="4f9af-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="4f9af-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="4f9af-122">isSubscribedByMail</span></span>
* <span data-ttu-id="4f9af-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="4f9af-123">unseenCount</span></span>

<span data-ttu-id="4f9af-p102">Para obter essas propriedades, use o parâmetro de consulta **$select**. Eis alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="4f9af-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="4f9af-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f9af-126">Permissions</span></span>
<span data-ttu-id="4f9af-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f9af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f9af-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f9af-129">Permission type</span></span>      | <span data-ttu-id="4f9af-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f9af-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f9af-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f9af-131">Delegated (work or school account)</span></span> | <span data-ttu-id="4f9af-132">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f9af-132">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f9af-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f9af-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f9af-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f9af-134">Not supported.</span></span>    |
|<span data-ttu-id="4f9af-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f9af-135">Application</span></span> | <span data-ttu-id="4f9af-136">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f9af-136">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f9af-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f9af-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f9af-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f9af-138">Optional query parameters</span></span>
<span data-ttu-id="4f9af-139">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f9af-139">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f9af-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f9af-140">Request headers</span></span>
| <span data-ttu-id="4f9af-141">Nome</span><span class="sxs-lookup"><span data-stu-id="4f9af-141">Name</span></span>       | <span data-ttu-id="4f9af-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f9af-142">Type</span></span> | <span data-ttu-id="4f9af-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f9af-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f9af-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f9af-144">Authorization</span></span>  | <span data-ttu-id="4f9af-145">string</span><span class="sxs-lookup"><span data-stu-id="4f9af-145">string</span></span>  | <span data-ttu-id="4f9af-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f9af-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f9af-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f9af-148">Request body</span></span>
<span data-ttu-id="4f9af-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f9af-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f9af-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f9af-150">Response</span></span>
<span data-ttu-id="4f9af-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f9af-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f9af-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f9af-152">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4f9af-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f9af-153">Request</span></span>
<span data-ttu-id="4f9af-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f9af-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="4f9af-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f9af-155">Response</span></span>
<span data-ttu-id="4f9af-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f9af-156">The following is an example of the response.</span></span>

><span data-ttu-id="4f9af-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f9af-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f9af-158">As propriedades padrão serão retornadas de uma chamada real, conforme descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="4f9af-158">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
