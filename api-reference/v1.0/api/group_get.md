# <a name="get-group"></a><span data-ttu-id="29db9-101">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="29db9-101">Get group</span></span>

<span data-ttu-id="29db9-102">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="29db9-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="29db9-103">Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="29db9-103">Default properties</span></span>

<span data-ttu-id="29db9-p101">O seguinte item representa o conjunto padrão de propriedades que são retornadas ao obter ou listar grupos. Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="29db9-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="29db9-106">descrição</span><span class="sxs-lookup"><span data-stu-id="29db9-106">description</span></span>
* <span data-ttu-id="29db9-107">displayName</span><span class="sxs-lookup"><span data-stu-id="29db9-107">displayName</span></span>
* <span data-ttu-id="29db9-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="29db9-108">groupTypes</span></span>
* <span data-ttu-id="29db9-109">id</span><span class="sxs-lookup"><span data-stu-id="29db9-109">id</span></span>
* <span data-ttu-id="29db9-110">Email</span><span class="sxs-lookup"><span data-stu-id="29db9-110">mail</span></span>
* <span data-ttu-id="29db9-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="29db9-111">mailEnabled</span></span>
* <span data-ttu-id="29db9-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="29db9-112">mailNickname</span></span>
* <span data-ttu-id="29db9-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="29db9-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="29db9-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="29db9-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="29db9-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="29db9-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="29db9-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="29db9-116">proxyAddresses</span></span>
* <span data-ttu-id="29db9-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="29db9-117">securityEnabled</span></span>
* <span data-ttu-id="29db9-118">visibilidade</span><span class="sxs-lookup"><span data-stu-id="29db9-118">visibility</span></span>

<span data-ttu-id="29db9-119">As seguintes propriedades de grupo não são retornadas por padrão:</span><span class="sxs-lookup"><span data-stu-id="29db9-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="29db9-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="29db9-120">allowExternalSenders</span></span>
* <span data-ttu-id="29db9-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="29db9-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="29db9-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="29db9-122">isSubscribedByMail</span></span>
* <span data-ttu-id="29db9-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="29db9-123">unseenCount</span></span>

<span data-ttu-id="29db9-p102">Para obter essas propriedades, use o parâmetro de consulta **$select**. Eis alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="29db9-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="prerequisites"></a><span data-ttu-id="29db9-126">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29db9-126">Prerequisites</span></span>
<span data-ttu-id="29db9-127">Um dos seguintes **escopos** é obrigatório para executar esta API: *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="29db9-127">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="29db9-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29db9-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29db9-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29db9-129">Optional query parameters</span></span>
<span data-ttu-id="29db9-130">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29db9-130">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29db9-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29db9-131">Request headers</span></span>
| <span data-ttu-id="29db9-132">Nome</span><span class="sxs-lookup"><span data-stu-id="29db9-132">Name</span></span>       | <span data-ttu-id="29db9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="29db9-133">Type</span></span> | <span data-ttu-id="29db9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="29db9-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29db9-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="29db9-135">Authorization</span></span>  | <span data-ttu-id="29db9-136">string</span><span class="sxs-lookup"><span data-stu-id="29db9-136">string</span></span>  | <span data-ttu-id="29db9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29db9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29db9-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29db9-139">Request body</span></span>
<span data-ttu-id="29db9-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29db9-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29db9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="29db9-141">Response</span></span>

<span data-ttu-id="29db9-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29db9-142">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29db9-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29db9-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29db9-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29db9-144">Request</span></span>
<span data-ttu-id="29db9-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29db9-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a><span data-ttu-id="29db9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="29db9-146">Response</span></span>
<span data-ttu-id="29db9-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29db9-147">Here is an example of the response.</span></span>

<span data-ttu-id="29db9-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. As propriedades padrão serão retornadas de uma chamada real, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="29db9-p104">Note: The response object shown here may be truncated for brevity. The default properties will be returned from an actual call, as described above.</span></span>
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
