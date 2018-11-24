# <a name="list-members"></a><span data-ttu-id="36c30-101">Listar membros</span><span class="sxs-lookup"><span data-stu-id="36c30-101">List members</span></span>

<span data-ttu-id="36c30-p101">Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="36c30-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="36c30-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="36c30-104">Permissions</span></span>
<span data-ttu-id="36c30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="36c30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="36c30-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36c30-107">Permission type</span></span>      | <span data-ttu-id="36c30-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36c30-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36c30-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36c30-109">Delegated (work or school account)</span></span> | <span data-ttu-id="36c30-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36c30-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36c30-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36c30-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36c30-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36c30-112">Not supported.</span></span>    |
|<span data-ttu-id="36c30-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36c30-113">Application</span></span> | <span data-ttu-id="36c30-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c30-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36c30-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36c30-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36c30-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36c30-116">Optional query parameters</span></span>
<span data-ttu-id="36c30-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36c30-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36c30-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36c30-118">Request headers</span></span>
| <span data-ttu-id="36c30-119">Nome</span><span class="sxs-lookup"><span data-stu-id="36c30-119">Name</span></span>       | <span data-ttu-id="36c30-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="36c30-120">Type</span></span> | <span data-ttu-id="36c30-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="36c30-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36c30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36c30-122">Authorization</span></span>  | <span data-ttu-id="36c30-123">string</span><span class="sxs-lookup"><span data-stu-id="36c30-123">string</span></span>  | <span data-ttu-id="36c30-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36c30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36c30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36c30-126">Request body</span></span>
<span data-ttu-id="36c30-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36c30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="36c30-128">Response</span></span>

<span data-ttu-id="36c30-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36c30-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36c30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36c30-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36c30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36c30-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="36c30-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="36c30-132">Response</span></span>
<span data-ttu-id="36c30-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36c30-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->