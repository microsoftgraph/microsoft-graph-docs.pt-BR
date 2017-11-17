# <a name="notebook-copynotebook"></a><span data-ttu-id="4b39f-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="4b39f-101">notebook: copyNotebook</span></span>
<span data-ttu-id="4b39f-p101">Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.</span><span class="sxs-lookup"><span data-stu-id="4b39f-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="4b39f-104">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="4b39f-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b39f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b39f-105">Permissions</span></span>
<span data-ttu-id="4b39f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b39f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b39f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b39f-108">Permission type</span></span>      | <span data-ttu-id="4b39f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b39f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b39f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b39f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b39f-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b39f-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b39f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b39f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b39f-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b39f-113">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b39f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b39f-114">Application</span></span> | <span data-ttu-id="4b39f-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b39f-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b39f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b39f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="4b39f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b39f-117">Request headers</span></span>
| <span data-ttu-id="4b39f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4b39f-118">Name</span></span>       | <span data-ttu-id="4b39f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b39f-119">Type</span></span> | <span data-ttu-id="4b39f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b39f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b39f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b39f-121">Authorization</span></span>  | <span data-ttu-id="4b39f-122">string</span><span class="sxs-lookup"><span data-stu-id="4b39f-122">string</span></span>  | <span data-ttu-id="4b39f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b39f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b39f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b39f-125">Content-Type</span></span> | <span data-ttu-id="4b39f-126">string</span><span class="sxs-lookup"><span data-stu-id="4b39f-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4b39f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b39f-127">Request body</span></span>
<span data-ttu-id="4b39f-p104">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa. É possível enviar um corpo vazio se nenhum objeto for necessário.</span><span class="sxs-lookup"><span data-stu-id="4b39f-p104">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="4b39f-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b39f-130">Parameter</span></span>    | <span data-ttu-id="4b39f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b39f-131">Type</span></span>   |<span data-ttu-id="4b39f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b39f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b39f-133">groupId</span><span class="sxs-lookup"><span data-stu-id="4b39f-133">groupId</span></span>|<span data-ttu-id="4b39f-134">String</span><span class="sxs-lookup"><span data-stu-id="4b39f-134">String</span></span>|<span data-ttu-id="4b39f-p105">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4b39f-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4b39f-137">renameAs</span><span class="sxs-lookup"><span data-stu-id="4b39f-137">renameAs</span></span>|<span data-ttu-id="4b39f-138">String</span><span class="sxs-lookup"><span data-stu-id="4b39f-138">String</span></span>|<span data-ttu-id="4b39f-p106">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="4b39f-p106">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="4b39f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b39f-141">Response</span></span>

<span data-ttu-id="4b39f-p107">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteOperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="4b39f-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4b39f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b39f-144">Example</span></span>
<span data-ttu-id="4b39f-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b39f-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b39f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b39f-146">Request</span></span>
<span data-ttu-id="4b39f-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b39f-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4b39f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b39f-148">Response</span></span>
<span data-ttu-id="4b39f-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b39f-149">Here is an example of the response.</span></span>
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
