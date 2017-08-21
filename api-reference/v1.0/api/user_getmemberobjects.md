# <a name="user-getmemberobjects"></a><span data-ttu-id="59534-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="59534-101">user: getMemberObjects</span></span>
<span data-ttu-id="59534-p101">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="59534-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59534-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59534-104">Prerequisites</span></span>
<span data-ttu-id="59534-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="59534-105">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="59534-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59534-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="59534-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59534-107">Request headers</span></span>
| <span data-ttu-id="59534-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59534-108">Header</span></span>       | <span data-ttu-id="59534-109">Valor</span><span class="sxs-lookup"><span data-stu-id="59534-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59534-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="59534-110">Authorization</span></span>  | <span data-ttu-id="59534-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59534-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59534-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59534-113">Content-Type</span></span>  | <span data-ttu-id="59534-114">application/json</span><span class="sxs-lookup"><span data-stu-id="59534-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59534-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59534-115">Request body</span></span>
<span data-ttu-id="59534-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59534-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59534-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59534-117">Parameter</span></span>    | <span data-ttu-id="59534-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="59534-118">Type</span></span>   |<span data-ttu-id="59534-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="59534-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59534-120">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="59534-120">securityEnabledOnly</span></span>|<span data-ttu-id="59534-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="59534-121">Boolean</span></span>|<span data-ttu-id="59534-p103">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="59534-p103">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="59534-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="59534-124">Response</span></span>

<span data-ttu-id="59534-125">Se bem-sucedido, este método retorna um código de resposta `200, OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="59534-125">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="59534-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59534-126">Example</span></span>
<span data-ttu-id="59534-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="59534-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59534-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59534-128">Request</span></span>
<span data-ttu-id="59534-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59534-129">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="59534-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="59534-130">Response</span></span>
<span data-ttu-id="59534-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59534-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
