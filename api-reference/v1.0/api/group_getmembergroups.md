# <a name="group-getmembergroups"></a><span data-ttu-id="0afb3-101">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0afb3-101">group: getMemberGroups</span></span>
<span data-ttu-id="0afb3-p101">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group_list_memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="0afb3-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="0afb3-p102">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="0afb3-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="0afb3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0afb3-108">Permissions</span></span>
<span data-ttu-id="0afb3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0afb3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0afb3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0afb3-111">Permission type</span></span>      | <span data-ttu-id="0afb3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0afb3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0afb3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0afb3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0afb3-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0afb3-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0afb3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0afb3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0afb3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0afb3-116">Not supported.</span></span>    |
|<span data-ttu-id="0afb3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0afb3-117">Application</span></span> | <span data-ttu-id="0afb3-118">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0afb3-118">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0afb3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0afb3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="0afb3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0afb3-120">Request headers</span></span>
| <span data-ttu-id="0afb3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0afb3-121">Name</span></span>       | <span data-ttu-id="0afb3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0afb3-122">Type</span></span> | <span data-ttu-id="0afb3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0afb3-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0afb3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0afb3-124">Authorization</span></span>  | <span data-ttu-id="0afb3-125">string</span><span class="sxs-lookup"><span data-stu-id="0afb3-125">string</span></span>  | <span data-ttu-id="0afb3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0afb3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0afb3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0afb3-128">Request body</span></span>
<span data-ttu-id="0afb3-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0afb3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0afb3-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0afb3-130">Parameter</span></span>    | <span data-ttu-id="0afb3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0afb3-131">Type</span></span>   |<span data-ttu-id="0afb3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0afb3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0afb3-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0afb3-133">securityEnabledOnly</span></span>|<span data-ttu-id="0afb3-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0afb3-134">Boolean</span></span>|<span data-ttu-id="0afb3-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="0afb3-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="0afb3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0afb3-137">Response</span></span>
<span data-ttu-id="0afb3-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="0afb3-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="0afb3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0afb3-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0afb3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0afb3-140">Request</span></span>
<span data-ttu-id="0afb3-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0afb3-141">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="0afb3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0afb3-142">Response</span></span>
<span data-ttu-id="0afb3-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0afb3-143">Here is an example of the response.</span></span>
><span data-ttu-id="0afb3-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0afb3-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0afb3-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0afb3-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
