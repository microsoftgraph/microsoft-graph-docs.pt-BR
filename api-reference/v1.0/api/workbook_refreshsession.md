# <a name="refresh-session"></a><span data-ttu-id="feaa5-101">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="feaa5-101">Refresh Session</span></span>

<span data-ttu-id="feaa5-102">Use esta API para atualizar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="feaa5-102">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="feaa5-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="feaa5-103">Permissions</span></span>
<span data-ttu-id="feaa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="feaa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="feaa5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feaa5-106">Permission type</span></span>      | <span data-ttu-id="feaa5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="feaa5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feaa5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feaa5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="feaa5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feaa5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="feaa5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feaa5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feaa5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feaa5-111">Not supported.</span></span>    |
|<span data-ttu-id="feaa5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feaa5-112">Application</span></span> | <span data-ttu-id="feaa5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feaa5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="feaa5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feaa5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="feaa5-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feaa5-115">Request headers</span></span>
| <span data-ttu-id="feaa5-116">Nome</span><span class="sxs-lookup"><span data-stu-id="feaa5-116">Name</span></span>       | <span data-ttu-id="feaa5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="feaa5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="feaa5-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="feaa5-118">Authorization</span></span>  | <span data-ttu-id="feaa5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feaa5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="feaa5-121">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="feaa5-121">workbook-session-id</span></span> | <span data-ttu-id="feaa5-122">Id de sessão de pasta de trabalho a ser atualizada</span><span class="sxs-lookup"><span data-stu-id="feaa5-122">Workbook session Id to be refreshd</span></span> |

## <a name="request-body"></a><span data-ttu-id="feaa5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feaa5-123">Request body</span></span>
<span data-ttu-id="feaa5-124">Esta API não exige o corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feaa5-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="feaa5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="feaa5-125">Response</span></span>

<span data-ttu-id="feaa5-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="feaa5-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="feaa5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feaa5-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="feaa5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feaa5-128">Request</span></span>
<span data-ttu-id="feaa5-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feaa5-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="feaa5-130">Observe que o cabeçalho workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="feaa5-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="feaa5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="feaa5-131">Response</span></span>
<span data-ttu-id="feaa5-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="feaa5-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```