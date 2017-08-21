# <a name="section-copytonotebook"></a><span data-ttu-id="efe04-101">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="efe04-101">section: copyToNotebook</span></span>
<span data-ttu-id="efe04-102">Copia uma seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="efe04-102">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="efe04-103">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e, em seguida, sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="efe04-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efe04-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efe04-104">Prerequisites</span></span>
<span data-ttu-id="efe04-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="efe04-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="efe04-106">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe04-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="efe04-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efe04-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="efe04-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efe04-108">Request headers</span></span>
| <span data-ttu-id="efe04-109">Nome</span><span class="sxs-lookup"><span data-stu-id="efe04-109">Name</span></span>       | <span data-ttu-id="efe04-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="efe04-110">Type</span></span> | <span data-ttu-id="efe04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="efe04-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efe04-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="efe04-112">Authorization</span></span>  | <span data-ttu-id="efe04-113">string</span><span class="sxs-lookup"><span data-stu-id="efe04-113">string</span></span>  | <span data-ttu-id="efe04-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efe04-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efe04-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efe04-116">Content-Type</span></span> | <span data-ttu-id="efe04-117">string</span><span class="sxs-lookup"><span data-stu-id="efe04-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="efe04-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efe04-118">Request body</span></span>
<span data-ttu-id="efe04-119">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="efe04-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="efe04-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="efe04-120">Parameter</span></span>    | <span data-ttu-id="efe04-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="efe04-121">Type</span></span>   |<span data-ttu-id="efe04-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="efe04-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe04-123">groupId</span><span class="sxs-lookup"><span data-stu-id="efe04-123">groupId</span></span>|<span data-ttu-id="efe04-124">String</span><span class="sxs-lookup"><span data-stu-id="efe04-124">String</span></span>|<span data-ttu-id="efe04-p102">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="efe04-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="efe04-127">id</span><span class="sxs-lookup"><span data-stu-id="efe04-127">id</span></span>|<span data-ttu-id="efe04-128">String</span><span class="sxs-lookup"><span data-stu-id="efe04-128">String</span></span>|<span data-ttu-id="efe04-p103">Obrigatório. A id do bloco de anotações de destino.</span><span class="sxs-lookup"><span data-stu-id="efe04-p103">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="efe04-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="efe04-131">renameAs</span></span>|<span data-ttu-id="efe04-132">String</span><span class="sxs-lookup"><span data-stu-id="efe04-132">String</span></span>|<span data-ttu-id="efe04-p104">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="efe04-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="efe04-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe04-135">Response</span></span>

<span data-ttu-id="efe04-p105">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="efe04-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="efe04-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efe04-138">Example</span></span>
<span data-ttu-id="efe04-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="efe04-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efe04-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efe04-140">Request</span></span>
<span data-ttu-id="efe04-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efe04-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="efe04-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="efe04-142">Response</span></span>
<span data-ttu-id="efe04-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efe04-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->