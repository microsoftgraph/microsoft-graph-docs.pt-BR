# <a name="group-getmemberobjects"></a><span data-ttu-id="276d6-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="276d6-101">group: getMemberObjects</span></span>
<span data-ttu-id="276d6-p101">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="276d6-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="276d6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="276d6-105">Permissions</span></span>
<span data-ttu-id="276d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="276d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="276d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="276d6-108">Permission type</span></span>      | <span data-ttu-id="276d6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="276d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="276d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="276d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="276d6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="276d6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="276d6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="276d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276d6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276d6-113">Not supported.</span></span>    |
|<span data-ttu-id="276d6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="276d6-114">Application</span></span> | <span data-ttu-id="276d6-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="276d6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="276d6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="276d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="276d6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="276d6-117">Request headers</span></span>
| <span data-ttu-id="276d6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="276d6-118">Name</span></span>       | <span data-ttu-id="276d6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="276d6-119">Type</span></span> | <span data-ttu-id="276d6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="276d6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="276d6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="276d6-121">Authorization</span></span>  | <span data-ttu-id="276d6-122">string</span><span class="sxs-lookup"><span data-stu-id="276d6-122">string</span></span>  | <span data-ttu-id="276d6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="276d6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="276d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="276d6-125">Request body</span></span>
<span data-ttu-id="276d6-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="276d6-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="276d6-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="276d6-127">Parameter</span></span>    | <span data-ttu-id="276d6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="276d6-128">Type</span></span>   |<span data-ttu-id="276d6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="276d6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="276d6-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="276d6-130">securityEnabledOnly</span></span>|<span data-ttu-id="276d6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="276d6-131">Boolean</span></span>| <span data-ttu-id="276d6-p104">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="276d6-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="276d6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="276d6-134">Response</span></span>
<span data-ttu-id="276d6-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="276d6-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="276d6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="276d6-136">Example</span></span>
<span data-ttu-id="276d6-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="276d6-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="276d6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="276d6-138">Request</span></span>
<span data-ttu-id="276d6-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="276d6-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="276d6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="276d6-140">Response</span></span>
<span data-ttu-id="276d6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="276d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
