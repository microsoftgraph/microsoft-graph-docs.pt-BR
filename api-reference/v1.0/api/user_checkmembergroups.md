# <a name="checkmembergroups"></a><span data-ttu-id="e81b1-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e81b1-101">checkMemberGroups</span></span>
<span data-ttu-id="e81b1-p101">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="e81b1-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="e81b1-p102">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="e81b1-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="e81b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e81b1-108">Prerequisites</span></span>
<span data-ttu-id="e81b1-109">Um dos seguintes **escopos** é necessário para executar esta API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="e81b1-109">One of the following **scopes** is required to execute this API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="e81b1-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e81b1-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="e81b1-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e81b1-111">Request headers</span></span>
| <span data-ttu-id="e81b1-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e81b1-112">Header</span></span>       | <span data-ttu-id="e81b1-113">Valor</span><span class="sxs-lookup"><span data-stu-id="e81b1-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e81b1-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="e81b1-114">Authorization</span></span>  | <span data-ttu-id="e81b1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e81b1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e81b1-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e81b1-117">Content-Type</span></span>  | <span data-ttu-id="e81b1-118">application/json</span><span class="sxs-lookup"><span data-stu-id="e81b1-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e81b1-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e81b1-119">Request body</span></span>
<span data-ttu-id="e81b1-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e81b1-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e81b1-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e81b1-121">Parameter</span></span>    | <span data-ttu-id="e81b1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e81b1-122">Type</span></span>   |<span data-ttu-id="e81b1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e81b1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e81b1-124">groupIds</span><span class="sxs-lookup"><span data-stu-id="e81b1-124">groupIds</span></span>|<span data-ttu-id="e81b1-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e81b1-125">String</span></span>|<span data-ttu-id="e81b1-126">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="e81b1-126">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="e81b1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e81b1-127">Response</span></span>

<span data-ttu-id="e81b1-128">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e81b1-128">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81b1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e81b1-129">Example</span></span>
<span data-ttu-id="e81b1-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e81b1-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e81b1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e81b1-131">Request</span></span>
<span data-ttu-id="e81b1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e81b1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e81b1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e81b1-133">Response</span></span>
<span data-ttu-id="e81b1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e81b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
