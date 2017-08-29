# <a name="user-getmemberobjects"></a><span data-ttu-id="4b416-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4b416-101">user: getMemberObjects</span></span>
<span data-ttu-id="4b416-p101">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="4b416-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b416-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b416-104">Permissions</span></span>
<span data-ttu-id="4b416-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b416-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4b416-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b416-107">Permission type</span></span>      | <span data-ttu-id="4b416-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b416-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b416-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b416-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4b416-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b416-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b416-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b416-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b416-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b416-112">Not supported.</span></span>    |
|<span data-ttu-id="4b416-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b416-113">Application</span></span> | <span data-ttu-id="4b416-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b416-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b416-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b416-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="4b416-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-116">Request headers</span></span>
| <span data-ttu-id="4b416-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b416-117">Header</span></span>       | <span data-ttu-id="4b416-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4b416-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b416-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b416-119">Authorization</span></span>  | <span data-ttu-id="4b416-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b416-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b416-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b416-122">Content-Type</span></span>  | <span data-ttu-id="4b416-123">application/json</span><span class="sxs-lookup"><span data-stu-id="4b416-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b416-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-124">Request body</span></span>
<span data-ttu-id="4b416-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b416-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b416-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b416-126">Parameter</span></span>    | <span data-ttu-id="4b416-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b416-127">Type</span></span>   |<span data-ttu-id="4b416-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b416-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b416-129">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4b416-129">securityEnabledOnly</span></span>|<span data-ttu-id="4b416-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b416-130">Boolean</span></span>|<span data-ttu-id="4b416-p104">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b416-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="4b416-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b416-133">Response</span></span>

<span data-ttu-id="4b416-134">Se bem-sucedido, este método retorna um código de resposta `200, OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="4b416-134">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="4b416-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b416-135">Example</span></span>
<span data-ttu-id="4b416-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b416-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b416-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-137">Request</span></span>
<span data-ttu-id="4b416-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b416-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="4b416-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b416-139">Response</span></span>
<span data-ttu-id="4b416-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b416-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
