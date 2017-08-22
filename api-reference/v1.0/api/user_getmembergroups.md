# <a name="user-getmembergroups"></a><span data-ttu-id="477a9-101">usuário: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="477a9-101">user: getMemberGroups</span></span>
<span data-ttu-id="477a9-p101">Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [member](../api/user_list_memberof.md), que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="477a9-p101">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user_list_memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="477a9-p102">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="477a9-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="477a9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="477a9-108">Prerequisites</span></span>
<span data-ttu-id="477a9-109">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read* ou *User.ReadBasic.All* e *Group.Read.All*; *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="477a9-109">One of the following **scopes** is required to execute this API: *User.Read* or *User.ReadBasic.All* and *Group.Read.All*; *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="477a9-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="477a9-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="477a9-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="477a9-111">Request headers</span></span>
| <span data-ttu-id="477a9-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="477a9-112">Header</span></span>       | <span data-ttu-id="477a9-113">Valor</span><span class="sxs-lookup"><span data-stu-id="477a9-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="477a9-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="477a9-114">Authorization</span></span>  | <span data-ttu-id="477a9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="477a9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="477a9-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="477a9-117">Content-Type</span></span>  | <span data-ttu-id="477a9-118">application/json</span><span class="sxs-lookup"><span data-stu-id="477a9-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="477a9-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="477a9-119">Request body</span></span>
<span data-ttu-id="477a9-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="477a9-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="477a9-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="477a9-121">Parameter</span></span>    | <span data-ttu-id="477a9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="477a9-122">Type</span></span>   |<span data-ttu-id="477a9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="477a9-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="477a9-124">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="477a9-124">securityEnabledOnly</span></span>|<span data-ttu-id="477a9-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="477a9-125">Boolean</span></span>|<span data-ttu-id="477a9-p104">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="477a9-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="477a9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="477a9-128">Response</span></span>

<span data-ttu-id="477a9-129">Se bem-sucedido, este método retorna um código de resposta `200, OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="477a9-129">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="477a9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="477a9-130">Example</span></span>
<span data-ttu-id="477a9-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="477a9-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="477a9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="477a9-132">Request</span></span>
<span data-ttu-id="477a9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="477a9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="477a9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="477a9-134">Response</span></span>
<span data-ttu-id="477a9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="477a9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
