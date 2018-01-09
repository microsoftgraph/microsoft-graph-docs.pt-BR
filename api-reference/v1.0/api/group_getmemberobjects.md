# <a name="group-getmemberobjects"></a><span data-ttu-id="c584c-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c584c-101">group: getMemberObjects</span></span>
<span data-ttu-id="c584c-p101">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="c584c-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c584c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c584c-105">Permissions</span></span>
<span data-ttu-id="c584c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c584c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c584c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c584c-108">Permission type</span></span>      | <span data-ttu-id="c584c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c584c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c584c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c584c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c584c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c584c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c584c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c584c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c584c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c584c-113">Not supported.</span></span>    |
|<span data-ttu-id="c584c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c584c-114">Application</span></span> | <span data-ttu-id="c584c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c584c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c584c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c584c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="c584c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c584c-117">Request headers</span></span>
| <span data-ttu-id="c584c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c584c-118">Name</span></span>       | <span data-ttu-id="c584c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c584c-119">Type</span></span> | <span data-ttu-id="c584c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c584c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c584c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c584c-121">Authorization</span></span>  | <span data-ttu-id="c584c-122">string</span><span class="sxs-lookup"><span data-stu-id="c584c-122">string</span></span>  | <span data-ttu-id="c584c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c584c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c584c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c584c-125">Request body</span></span>
<span data-ttu-id="c584c-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c584c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c584c-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c584c-127">Parameter</span></span>    | <span data-ttu-id="c584c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c584c-128">Type</span></span>   |<span data-ttu-id="c584c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c584c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c584c-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c584c-130">securityEnabledOnly</span></span>|<span data-ttu-id="c584c-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c584c-131">Boolean</span></span>| <span data-ttu-id="c584c-p104">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="c584c-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="c584c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c584c-134">Response</span></span>
<span data-ttu-id="c584c-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="c584c-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="c584c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c584c-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c584c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c584c-137">Request</span></span>
<span data-ttu-id="c584c-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c584c-138">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="c584c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c584c-139">Response</span></span>
<span data-ttu-id="c584c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c584c-140">Here is an example of the response.</span></span>
><span data-ttu-id="c584c-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c584c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c584c-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c584c-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
