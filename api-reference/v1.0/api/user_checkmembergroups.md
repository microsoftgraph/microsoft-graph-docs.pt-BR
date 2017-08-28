# <a name="checkmembergroups"></a><span data-ttu-id="3a9f1-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3a9f1-101">checkMemberGroups</span></span>
<span data-ttu-id="3a9f1-p101">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="3a9f1-p102">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3a9f1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a9f1-108">Permissions</span></span>
<span data-ttu-id="3a9f1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a9f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a9f1-111">Permission type</span></span>      | <span data-ttu-id="3a9f1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a9f1-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3a9f1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a9f1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a9f1-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a9f1-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="3a9f1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a9f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a9f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-116">Not supported.</span></span>    | 
|<span data-ttu-id="3a9f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a9f1-117">Application</span></span> | <span data-ttu-id="3a9f1-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9f1-118">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a9f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9f1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="3a9f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9f1-120">Request headers</span></span>
| <span data-ttu-id="3a9f1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a9f1-121">Header</span></span>       | <span data-ttu-id="3a9f1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a9f1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a9f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a9f1-123">Authorization</span></span>  | <span data-ttu-id="3a9f1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a9f1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a9f1-126">Content-Type</span></span>  | <span data-ttu-id="3a9f1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9f1-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a9f1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9f1-128">Request body</span></span>
<span data-ttu-id="3a9f1-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a9f1-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a9f1-130">Parameter</span></span>    | <span data-ttu-id="3a9f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a9f1-131">Type</span></span>   |<span data-ttu-id="3a9f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a9f1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a9f1-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="3a9f1-133">groupIds</span></span>|<span data-ttu-id="3a9f1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a9f1-134">String</span></span>|<span data-ttu-id="3a9f1-135">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="3a9f1-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="3a9f1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9f1-136">Response</span></span>

<span data-ttu-id="3a9f1-137">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-137">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9f1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a9f1-138">Example</span></span>
<span data-ttu-id="3a9f1-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a9f1-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9f1-140">Request</span></span>
<span data-ttu-id="3a9f1-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3a9f1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9f1-142">Response</span></span>
<span data-ttu-id="3a9f1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a9f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
