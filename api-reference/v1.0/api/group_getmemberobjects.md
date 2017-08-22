# <a name="group-getmemberobjects"></a><span data-ttu-id="e8456-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e8456-101">group: getMemberObjects</span></span>
<span data-ttu-id="e8456-p101">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="e8456-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8456-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8456-105">Prerequisites</span></span>
<span data-ttu-id="e8456-106">Um dos seguintes **escopos** é obrigatório para executar esta API: Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="e8456-106">One of the following **scopes** is required to execute this API: One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e8456-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8456-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="e8456-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8456-108">Request headers</span></span>
| <span data-ttu-id="e8456-109">Nome</span><span class="sxs-lookup"><span data-stu-id="e8456-109">Name</span></span>       | <span data-ttu-id="e8456-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8456-110">Type</span></span> | <span data-ttu-id="e8456-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8456-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8456-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8456-112">Authorization</span></span>  | <span data-ttu-id="e8456-113">string</span><span class="sxs-lookup"><span data-stu-id="e8456-113">string</span></span>  | <span data-ttu-id="e8456-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8456-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8456-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8456-116">Request body</span></span>
<span data-ttu-id="e8456-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8456-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8456-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8456-118">Parameter</span></span>    | <span data-ttu-id="e8456-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8456-119">Type</span></span>   |<span data-ttu-id="e8456-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8456-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8456-121">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e8456-121">securityEnabledOnly</span></span>|<span data-ttu-id="e8456-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8456-122">Boolean</span></span>| <span data-ttu-id="e8456-p103">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="e8456-p103">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="e8456-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8456-125">Response</span></span>

<span data-ttu-id="e8456-126">Se bem-sucedido, este método retorna um código de resposta `200, OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="e8456-126">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="e8456-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8456-127">Example</span></span>
<span data-ttu-id="e8456-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e8456-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8456-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8456-129">Request</span></span>
<span data-ttu-id="e8456-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8456-130">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e8456-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8456-131">Response</span></span>
<span data-ttu-id="e8456-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8456-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
