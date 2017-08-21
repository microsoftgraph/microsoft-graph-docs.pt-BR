# <a name="page-copytosection"></a><span data-ttu-id="0efea-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="0efea-101">page: copyToSection</span></span>
<span data-ttu-id="0efea-102">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="0efea-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="0efea-103">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e, em seguida, sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="0efea-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0efea-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0efea-104">Prerequisites</span></span>
<span data-ttu-id="0efea-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="0efea-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="0efea-106">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0efea-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>  

## <a name="http-request"></a><span data-ttu-id="0efea-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0efea-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="0efea-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0efea-108">Request headers</span></span>
| <span data-ttu-id="0efea-109">Nome</span><span class="sxs-lookup"><span data-stu-id="0efea-109">Name</span></span>       | <span data-ttu-id="0efea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efea-110">Type</span></span> | <span data-ttu-id="0efea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efea-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0efea-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="0efea-112">Authorization</span></span>  | <span data-ttu-id="0efea-113">string</span><span class="sxs-lookup"><span data-stu-id="0efea-113">string</span></span>  | <span data-ttu-id="0efea-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0efea-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0efea-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0efea-116">Content-Type</span></span> | <span data-ttu-id="0efea-117">string</span><span class="sxs-lookup"><span data-stu-id="0efea-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0efea-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0efea-118">Request body</span></span>
<span data-ttu-id="0efea-119">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="0efea-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="0efea-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0efea-120">Parameter</span></span>    | <span data-ttu-id="0efea-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efea-121">Type</span></span>   |<span data-ttu-id="0efea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efea-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0efea-123">groupId</span><span class="sxs-lookup"><span data-stu-id="0efea-123">groupId</span></span>|<span data-ttu-id="0efea-124">String</span><span class="sxs-lookup"><span data-stu-id="0efea-124">String</span></span>|<span data-ttu-id="0efea-p102">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="0efea-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="0efea-127">id</span><span class="sxs-lookup"><span data-stu-id="0efea-127">id</span></span>|<span data-ttu-id="0efea-128">String</span><span class="sxs-lookup"><span data-stu-id="0efea-128">String</span></span>|<span data-ttu-id="0efea-p103">Obrigatório. A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="0efea-p103">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="0efea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0efea-131">Response</span></span>

<span data-ttu-id="0efea-p104">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="0efea-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="0efea-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0efea-134">Example</span></span>
<span data-ttu-id="0efea-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0efea-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0efea-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0efea-136">Request</span></span>
<span data-ttu-id="0efea-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0efea-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="0efea-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0efea-138">Response</span></span>
<span data-ttu-id="0efea-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0efea-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->