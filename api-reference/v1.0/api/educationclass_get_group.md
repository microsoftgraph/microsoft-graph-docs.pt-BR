# <a name="get-group"></a><span data-ttu-id="a5ce7-101">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="a5ce7-101">Get group</span></span>

<span data-ttu-id="a5ce7-102">Recupere o **group** do Office 365 que corresponde a essa **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-102">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="a5ce7-103">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="a5ce7-104">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ce7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5ce7-105">Permissions</span></span>
<span data-ttu-id="a5ce7-106">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="a5ce7-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5ce7-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5ce7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5ce7-108">Permission type</span></span>      | <span data-ttu-id="a5ce7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5ce7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5ce7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5ce7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5ce7-111">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ce7-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="a5ce7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5ce7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5ce7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-113">Not supported.</span></span>  |
|<span data-ttu-id="a5ce7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5ce7-114">Application</span></span> | <span data-ttu-id="a5ce7-115">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ce7-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="a5ce7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ce7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="a5ce7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ce7-117">Request headers</span></span>
| <span data-ttu-id="a5ce7-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5ce7-118">Header</span></span>       | <span data-ttu-id="a5ce7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a5ce7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5ce7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5ce7-120">Authorization</span></span>  | <span data-ttu-id="a5ce7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5ce7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ce7-123">Request body</span></span>
<span data-ttu-id="a5ce7-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a5ce7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ce7-125">Response</span></span>
<span data-ttu-id="a5ce7-126">Se bem-sucedido, esse método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-126">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5ce7-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5ce7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5ce7-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ce7-128">Request</span></span>
<span data-ttu-id="a5ce7-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="a5ce7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ce7-130">Response</span></span>
<span data-ttu-id="a5ce7-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-131">The following is an example of the response.</span></span> 

><span data-ttu-id="a5ce7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ce7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
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

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->