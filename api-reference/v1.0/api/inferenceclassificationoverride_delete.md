# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="079f8-101">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="079f8-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="079f8-102">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="079f8-102">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="079f8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="079f8-103">Permissions</span></span>
<span data-ttu-id="079f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="079f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="079f8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="079f8-106">Permission type</span></span>      | <span data-ttu-id="079f8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="079f8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="079f8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="079f8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="079f8-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="079f8-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="079f8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="079f8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="079f8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="079f8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="079f8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="079f8-112">Application</span></span> | <span data-ttu-id="079f8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="079f8-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="079f8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="079f8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="079f8-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="079f8-115">Request headers</span></span>
| <span data-ttu-id="079f8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="079f8-116">Name</span></span>       | <span data-ttu-id="079f8-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="079f8-117">Type</span></span> | <span data-ttu-id="079f8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="079f8-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="079f8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="079f8-119">Authorization</span></span>  | <span data-ttu-id="079f8-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="079f8-120">string</span></span>  | <span data-ttu-id="079f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="079f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="079f8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="079f8-123">Request body</span></span>
<span data-ttu-id="079f8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="079f8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="079f8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="079f8-125">Response</span></span>

<span data-ttu-id="079f8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="079f8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="079f8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="079f8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="079f8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="079f8-129">Request</span></span>
<span data-ttu-id="079f8-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="079f8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="079f8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="079f8-131">Response</span></span>
<span data-ttu-id="079f8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="079f8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->