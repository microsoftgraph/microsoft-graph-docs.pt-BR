# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="a3599-101">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="a3599-101">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="a3599-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="a3599-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="a3599-104">**Observação**</span><span class="sxs-lookup"><span data-stu-id="a3599-104">**Note**</span></span>

- <span data-ttu-id="a3599-105">Se já existir uma substituição com o mesmo endereço STMP, os campos **classifyAs** e **name** da substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="a3599-105">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="a3599-106">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="a3599-106">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="a3599-107">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="a3599-107">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3599-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3599-108">Permissions</span></span>
<span data-ttu-id="a3599-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3599-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a3599-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3599-111">Permission type</span></span>      | <span data-ttu-id="a3599-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3599-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3599-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3599-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a3599-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3599-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a3599-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3599-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3599-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3599-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a3599-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3599-117">Application</span></span> | <span data-ttu-id="a3599-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3599-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3599-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3599-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="a3599-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3599-120">Request headers</span></span>
| <span data-ttu-id="a3599-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a3599-121">Name</span></span>       | <span data-ttu-id="a3599-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3599-122">Type</span></span> | <span data-ttu-id="a3599-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3599-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3599-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3599-124">Authorization</span></span>  | <span data-ttu-id="a3599-125">string</span><span class="sxs-lookup"><span data-stu-id="a3599-125">string</span></span>  | <span data-ttu-id="a3599-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3599-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3599-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3599-128">Content-Type</span></span> | <span data-ttu-id="a3599-129">string</span><span class="sxs-lookup"><span data-stu-id="a3599-129">string</span></span>  | <span data-ttu-id="a3599-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3599-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3599-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3599-132">Request body</span></span>
<span data-ttu-id="a3599-133">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="a3599-133">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a3599-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3599-134">Response</span></span>

<span data-ttu-id="a3599-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3599-135">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3599-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3599-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3599-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3599-137">Request</span></span>
<span data-ttu-id="a3599-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3599-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a3599-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3599-139">Response</span></span>
<span data-ttu-id="a3599-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3599-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->