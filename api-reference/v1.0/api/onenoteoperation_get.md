# <a name="get-onenoteoperation"></a><span data-ttu-id="af4dc-101">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="af4dc-101">Get onenoteOperation</span></span>

<span data-ttu-id="af4dc-p101">Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="af4dc-p101">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="af4dc-104">Você pode sondar o ponto de extremidade de Operation-Location até a propriedade `status` retornar `completed` ou `failed`.</span><span class="sxs-lookup"><span data-stu-id="af4dc-104">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="af4dc-105">Se o status for `completed`, a propriedade `resourceLocation` conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="af4dc-105">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="af4dc-106">Se o status for `failed`, o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="af4dc-106">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="af4dc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="af4dc-107">Permissions</span></span>
<span data-ttu-id="af4dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af4dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af4dc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af4dc-110">Permission type</span></span>      | <span data-ttu-id="af4dc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af4dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af4dc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af4dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af4dc-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af4dc-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="af4dc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af4dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af4dc-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af4dc-115">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="af4dc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af4dc-116">Application</span></span> | <span data-ttu-id="af4dc-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af4dc-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af4dc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af4dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af4dc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af4dc-119">Optional query parameters</span></span>
<span data-ttu-id="af4dc-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af4dc-120">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af4dc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af4dc-121">Request headers</span></span>
| <span data-ttu-id="af4dc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="af4dc-122">Name</span></span>       | <span data-ttu-id="af4dc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="af4dc-123">Type</span></span> | <span data-ttu-id="af4dc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="af4dc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af4dc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="af4dc-125">Authorization</span></span>  | <span data-ttu-id="af4dc-126">string</span><span class="sxs-lookup"><span data-stu-id="af4dc-126">string</span></span>  | <span data-ttu-id="af4dc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af4dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af4dc-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af4dc-129">Accept</span></span> | <span data-ttu-id="af4dc-130">string</span><span class="sxs-lookup"><span data-stu-id="af4dc-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="af4dc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af4dc-131">Request body</span></span>
<span data-ttu-id="af4dc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af4dc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af4dc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af4dc-133">Response</span></span>

<span data-ttu-id="af4dc-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af4dc-134">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af4dc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af4dc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af4dc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af4dc-136">Request</span></span>
<span data-ttu-id="af4dc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af4dc-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="af4dc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="af4dc-138">Response</span></span>
<span data-ttu-id="af4dc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af4dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
