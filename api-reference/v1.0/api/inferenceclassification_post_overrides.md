# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="2006a-101">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2006a-101">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="2006a-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="2006a-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="2006a-104">**Observação**</span><span class="sxs-lookup"><span data-stu-id="2006a-104">**Note**</span></span>

- <span data-ttu-id="2006a-105">Se já existir uma substituição com o mesmo endereço STMP, os campos **classifyAs** e **name** da substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="2006a-105">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="2006a-106">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="2006a-106">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="2006a-107">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="2006a-107">The POST operation supports creating only one override at a time.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2006a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2006a-108">Prerequisites</span></span>
<span data-ttu-id="2006a-109">Os seguintes **escopos** são necessários para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2006a-109">The following **scopes** are required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2006a-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2006a-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="2006a-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2006a-111">Request headers</span></span>
| <span data-ttu-id="2006a-112">Nome</span><span class="sxs-lookup"><span data-stu-id="2006a-112">Name</span></span>       | <span data-ttu-id="2006a-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="2006a-113">Type</span></span> | <span data-ttu-id="2006a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2006a-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2006a-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="2006a-115">Authorization</span></span>  | <span data-ttu-id="2006a-116">string</span><span class="sxs-lookup"><span data-stu-id="2006a-116">string</span></span>  | <span data-ttu-id="2006a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2006a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2006a-119">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2006a-119">Content-Type</span></span> | <span data-ttu-id="2006a-120">string</span><span class="sxs-lookup"><span data-stu-id="2006a-120">string</span></span>  | <span data-ttu-id="2006a-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2006a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2006a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2006a-123">Request body</span></span>
<span data-ttu-id="2006a-124">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="2006a-124">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2006a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2006a-125">Response</span></span>

<span data-ttu-id="2006a-126">Se for bem-sucedido, este método retornará um código de resposta `201, Created` e um objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2006a-126">If successful, this method returns `201, Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2006a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2006a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2006a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2006a-128">Request</span></span>
<span data-ttu-id="2006a-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2006a-129">Here is an example of the request.</span></span>
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
    "name": "Fanny Downs",
    "address": "fannyd@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="2006a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2006a-130">Response</span></span>
<span data-ttu-id="2006a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2006a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "name": "Fanny Downs",
    "address": "fannyd@adatum.onmicrosoft.com"
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