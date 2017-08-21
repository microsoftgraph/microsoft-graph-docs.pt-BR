# <a name="notebook-copynotebook"></a><span data-ttu-id="abba7-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="abba7-101">notebook: copyNotebook</span></span>
<span data-ttu-id="abba7-p101">Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.</span><span class="sxs-lookup"><span data-stu-id="abba7-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="abba7-104">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e, em seguida, sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="abba7-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abba7-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abba7-105">Prerequisites</span></span>
<span data-ttu-id="abba7-106">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="abba7-106">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="abba7-107">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abba7-107">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="abba7-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abba7-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="abba7-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abba7-109">Request headers</span></span>
| <span data-ttu-id="abba7-110">Nome</span><span class="sxs-lookup"><span data-stu-id="abba7-110">Name</span></span>       | <span data-ttu-id="abba7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="abba7-111">Type</span></span> | <span data-ttu-id="abba7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="abba7-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="abba7-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="abba7-113">Authorization</span></span>  | <span data-ttu-id="abba7-114">string</span><span class="sxs-lookup"><span data-stu-id="abba7-114">string</span></span>  | <span data-ttu-id="abba7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abba7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="abba7-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abba7-117">Content-Type</span></span> | <span data-ttu-id="abba7-118">string</span><span class="sxs-lookup"><span data-stu-id="abba7-118">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="abba7-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abba7-119">Request body</span></span>
<span data-ttu-id="abba7-p103">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa. É possível enviar um corpo vazio se nenhum objeto for necessário.</span><span class="sxs-lookup"><span data-stu-id="abba7-p103">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="abba7-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="abba7-122">Parameter</span></span>    | <span data-ttu-id="abba7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="abba7-123">Type</span></span>   |<span data-ttu-id="abba7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="abba7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abba7-125">groupId</span><span class="sxs-lookup"><span data-stu-id="abba7-125">groupId</span></span>|<span data-ttu-id="abba7-126">String</span><span class="sxs-lookup"><span data-stu-id="abba7-126">String</span></span>|<span data-ttu-id="abba7-p104">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="abba7-p104">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="abba7-129">renameAs</span><span class="sxs-lookup"><span data-stu-id="abba7-129">renameAs</span></span>|<span data-ttu-id="abba7-130">String</span><span class="sxs-lookup"><span data-stu-id="abba7-130">String</span></span>|<span data-ttu-id="abba7-p105">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="abba7-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="abba7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="abba7-133">Response</span></span>

<span data-ttu-id="abba7-p106">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteOperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="abba7-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="abba7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abba7-136">Example</span></span>
<span data-ttu-id="abba7-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="abba7-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="abba7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abba7-138">Request</span></span>
<span data-ttu-id="abba7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abba7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="abba7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="abba7-140">Response</span></span>
<span data-ttu-id="abba7-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abba7-141">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
