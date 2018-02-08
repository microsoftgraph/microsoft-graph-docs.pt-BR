# <a name="group-checkmembergroups"></a><span data-ttu-id="f1e46-101">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f1e46-101">group: checkMemberGroups</span></span>
<span data-ttu-id="f1e46-p101">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="f1e46-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span> 

<span data-ttu-id="f1e46-p102">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="f1e46-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f1e46-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1e46-108">Permissions</span></span>
<span data-ttu-id="f1e46-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1e46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="f1e46-111">**Observação:** esta API atualmente exige permissão Directory.Read.All ou posterior.</span><span class="sxs-lookup"><span data-stu-id="f1e46-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="f1e46-112">Usar a permissão Group.Read.All retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="f1e46-112">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="f1e46-113">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="f1e46-113">This is a known bug.</span></span>

|<span data-ttu-id="f1e46-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1e46-114">Permission type</span></span>      | <span data-ttu-id="f1e46-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1e46-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|

<span data-ttu-id="f1e46-116">|Delegado (conta corporativa ou de estudante) | *Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All | |Delegado (conta pessoal da Microsoft) | Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1e46-116">|Delegated (work or school account) | *Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All | |Delegated (personal Microsoft account) | Not supported.</span></span>    <span data-ttu-id="f1e46-117">| | Aplicativo | *Group.Read.All*, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="f1e46-117">| |Application | *Group.Read.All*, Directory.Read.All.</span></span> <span data-ttu-id="f1e46-118">Directory.ReadWrite.All |</span><span class="sxs-lookup"><span data-stu-id="f1e46-118">Directory.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f1e46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1e46-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="f1e46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e46-120">Request headers</span></span>
| <span data-ttu-id="f1e46-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f1e46-121">Name</span></span>       | <span data-ttu-id="f1e46-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1e46-122">Type</span></span> | <span data-ttu-id="f1e46-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1e46-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1e46-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1e46-124">Authorization</span></span>  | <span data-ttu-id="f1e46-125">string</span><span class="sxs-lookup"><span data-stu-id="f1e46-125">string</span></span>  | <span data-ttu-id="f1e46-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1e46-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1e46-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e46-128">Request body</span></span>
<span data-ttu-id="f1e46-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1e46-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1e46-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1e46-130">Parameter</span></span>    | <span data-ttu-id="f1e46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1e46-131">Type</span></span>   |<span data-ttu-id="f1e46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1e46-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1e46-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="f1e46-133">groupIds</span></span>|<span data-ttu-id="f1e46-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1e46-134">String</span></span>|<span data-ttu-id="f1e46-135">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="f1e46-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="f1e46-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e46-136">Response</span></span>

<span data-ttu-id="f1e46-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1e46-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e46-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1e46-138">Example</span></span>
<span data-ttu-id="f1e46-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f1e46-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1e46-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e46-140">Request</span></span>
<span data-ttu-id="f1e46-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1e46-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f1e46-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e46-142">Response</span></span>
<span data-ttu-id="f1e46-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1e46-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
