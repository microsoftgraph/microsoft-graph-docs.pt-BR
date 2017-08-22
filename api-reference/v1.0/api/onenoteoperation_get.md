# <a name="get-onenoteoperation"></a><span data-ttu-id="cad80-101">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="cad80-101">Get onenoteOperation</span></span>

<span data-ttu-id="cad80-p101">Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="cad80-p101">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="cad80-104">Você pode sondar o ponto de extremidade de Operation-Location até a propriedade `status` retornar `completed` ou `failed`.</span><span class="sxs-lookup"><span data-stu-id="cad80-104">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="cad80-105">Se o status for `completed`, a propriedade `resourceLocation` conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="cad80-105">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="cad80-106">Se o status for `failed`, o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="cad80-106">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cad80-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cad80-107">Prerequisites</span></span>
<span data-ttu-id="cad80-108">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="cad80-108">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="cad80-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad80-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>  

## <a name="http-request"></a><span data-ttu-id="cad80-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cad80-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cad80-111">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cad80-111">Optional query parameters</span></span>
<span data-ttu-id="cad80-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad80-112">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cad80-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cad80-113">Request headers</span></span>
| <span data-ttu-id="cad80-114">Nome</span><span class="sxs-lookup"><span data-stu-id="cad80-114">Name</span></span>       | <span data-ttu-id="cad80-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="cad80-115">Type</span></span> | <span data-ttu-id="cad80-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad80-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cad80-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="cad80-117">Authorization</span></span>  | <span data-ttu-id="cad80-118">string</span><span class="sxs-lookup"><span data-stu-id="cad80-118">string</span></span>  | <span data-ttu-id="cad80-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cad80-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cad80-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cad80-121">Accept</span></span> | <span data-ttu-id="cad80-122">string</span><span class="sxs-lookup"><span data-stu-id="cad80-122">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="cad80-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cad80-123">Request body</span></span>
<span data-ttu-id="cad80-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cad80-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cad80-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad80-125">Response</span></span>

<span data-ttu-id="cad80-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cad80-126">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cad80-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cad80-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cad80-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cad80-128">Request</span></span>
<span data-ttu-id="cad80-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cad80-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="cad80-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad80-130">Response</span></span>
<span data-ttu-id="cad80-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cad80-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
