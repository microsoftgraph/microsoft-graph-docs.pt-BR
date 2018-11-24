# <a name="list-directoryroles"></a><span data-ttu-id="ef15b-101">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="ef15b-101">List directoryRoles</span></span>

<span data-ttu-id="ef15b-102">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="ef15b-102">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef15b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef15b-103">Permissions</span></span>
<span data-ttu-id="ef15b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef15b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef15b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef15b-106">Permission type</span></span>      | <span data-ttu-id="ef15b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef15b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef15b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef15b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ef15b-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef15b-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef15b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef15b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef15b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef15b-111">Not supported.</span></span>    |
|<span data-ttu-id="ef15b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef15b-112">Application</span></span> | <span data-ttu-id="ef15b-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef15b-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef15b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef15b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef15b-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ef15b-115">Optional query parameters</span></span>
<span data-ttu-id="ef15b-116">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="ef15b-116">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef15b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef15b-117">Request headers</span></span>
| <span data-ttu-id="ef15b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ef15b-118">Name</span></span>       | <span data-ttu-id="ef15b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef15b-119">Type</span></span> | <span data-ttu-id="ef15b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef15b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef15b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef15b-121">Authorization</span></span>  | <span data-ttu-id="ef15b-122">string</span><span class="sxs-lookup"><span data-stu-id="ef15b-122">string</span></span>  | <span data-ttu-id="ef15b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef15b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef15b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef15b-125">Request body</span></span>
<span data-ttu-id="ef15b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef15b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef15b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef15b-127">Response</span></span>

<span data-ttu-id="ef15b-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef15b-128">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef15b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef15b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef15b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef15b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="ef15b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef15b-131">Response</span></span>
<span data-ttu-id="ef15b-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef15b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
