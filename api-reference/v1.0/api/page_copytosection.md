# <a name="page-copytosection"></a><span data-ttu-id="f5715-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="f5715-101">page: copyToSection</span></span>
<span data-ttu-id="f5715-102">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="f5715-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="f5715-103">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="f5715-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5715-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5715-104">Permissions</span></span>
<span data-ttu-id="f5715-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5715-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5715-107">Permission type</span></span>      | <span data-ttu-id="f5715-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5715-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f5715-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5715-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f5715-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5715-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f5715-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5715-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5715-112">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5715-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f5715-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5715-113">Application</span></span> | <span data-ttu-id="f5715-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5715-114">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f5715-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5715-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="f5715-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5715-116">Request headers</span></span>
| <span data-ttu-id="f5715-117">Nome</span><span class="sxs-lookup"><span data-stu-id="f5715-117">Name</span></span>       | <span data-ttu-id="f5715-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5715-118">Type</span></span> | <span data-ttu-id="f5715-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5715-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5715-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5715-120">Authorization</span></span>  | <span data-ttu-id="f5715-121">string</span><span class="sxs-lookup"><span data-stu-id="f5715-121">string</span></span>  | <span data-ttu-id="f5715-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5715-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5715-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5715-124">Content-Type</span></span> | <span data-ttu-id="f5715-125">string</span><span class="sxs-lookup"><span data-stu-id="f5715-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f5715-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5715-126">Request body</span></span>
<span data-ttu-id="f5715-127">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="f5715-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="f5715-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f5715-128">Parameter</span></span>    | <span data-ttu-id="f5715-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5715-129">Type</span></span>   |<span data-ttu-id="f5715-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5715-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5715-131">groupId</span><span class="sxs-lookup"><span data-stu-id="f5715-131">groupId</span></span>|<span data-ttu-id="f5715-132">String</span><span class="sxs-lookup"><span data-stu-id="f5715-132">String</span></span>|<span data-ttu-id="f5715-p103">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f5715-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="f5715-135">id</span><span class="sxs-lookup"><span data-stu-id="f5715-135">id</span></span>|<span data-ttu-id="f5715-136">String</span><span class="sxs-lookup"><span data-stu-id="f5715-136">String</span></span>|<span data-ttu-id="f5715-p104">Obrigatório. A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="f5715-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="f5715-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5715-139">Response</span></span>

<span data-ttu-id="f5715-p105">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="f5715-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="f5715-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5715-142">Example</span></span>
<span data-ttu-id="f5715-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f5715-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5715-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5715-144">Request</span></span>
<span data-ttu-id="f5715-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5715-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f5715-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5715-146">Response</span></span>
<span data-ttu-id="f5715-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5715-147">Here is an example of the response.</span></span>
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