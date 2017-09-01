# <a name="filter-apply"></a><span data-ttu-id="b809a-101">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="b809a-101">Filter: apply</span></span>

<span data-ttu-id="b809a-102">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="b809a-102">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="b809a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b809a-103">Permissions</span></span>
<span data-ttu-id="b809a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b809a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b809a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b809a-106">Permission type</span></span>      | <span data-ttu-id="b809a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b809a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b809a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b809a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b809a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b809a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b809a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b809a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b809a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b809a-111">Not supported.</span></span>    |
|<span data-ttu-id="b809a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b809a-112">Application</span></span> | <span data-ttu-id="b809a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b809a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b809a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b809a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="b809a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b809a-115">Request headers</span></span>
| <span data-ttu-id="b809a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b809a-116">Name</span></span>       | <span data-ttu-id="b809a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b809a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b809a-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b809a-118">Authorization</span></span>  | <span data-ttu-id="b809a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b809a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b809a-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b809a-121">Request body</span></span>
<span data-ttu-id="b809a-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b809a-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b809a-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b809a-123">Parameter</span></span>    | <span data-ttu-id="b809a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b809a-124">Type</span></span>   |<span data-ttu-id="b809a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b809a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b809a-126">critérios</span><span class="sxs-lookup"><span data-stu-id="b809a-126">criteria</span></span>|<span data-ttu-id="b809a-127">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="b809a-127">FilterCriteria</span></span>|<span data-ttu-id="b809a-128">Os critérios a aplicar.</span><span class="sxs-lookup"><span data-stu-id="b809a-128">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="b809a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b809a-129">Response</span></span>

<span data-ttu-id="b809a-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b809a-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b809a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b809a-132">Example</span></span>
<span data-ttu-id="b809a-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b809a-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b809a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b809a-134">Request</span></span>
<span data-ttu-id="b809a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b809a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="b809a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b809a-136">Response</span></span>
<span data-ttu-id="b809a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b809a-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->