# <a name="list-overrides"></a><span data-ttu-id="1460c-101">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="1460c-101">List overrides</span></span>

<span data-ttu-id="1460c-102">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="1460c-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="1460c-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="1460c-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1460c-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1460c-105">Prerequisites</span></span>
<span data-ttu-id="1460c-106">Os seguintes **escopos** são necessários para executar esta API: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="1460c-106">The following **scopes** are required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="1460c-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1460c-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="1460c-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1460c-108">Request headers</span></span>
| <span data-ttu-id="1460c-109">Nome</span><span class="sxs-lookup"><span data-stu-id="1460c-109">Name</span></span>       | <span data-ttu-id="1460c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1460c-110">Type</span></span> | <span data-ttu-id="1460c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1460c-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1460c-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="1460c-112">Authorization</span></span>  | <span data-ttu-id="1460c-113">string</span><span class="sxs-lookup"><span data-stu-id="1460c-113">string</span></span>  | <span data-ttu-id="1460c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1460c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1460c-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1460c-116">Request body</span></span>
<span data-ttu-id="1460c-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1460c-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1460c-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="1460c-118">Response</span></span>

<span data-ttu-id="1460c-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta. Retorna uma coleção vazia se o usuário não tiver quaisquer substituições configuradas.</span><span class="sxs-lookup"><span data-stu-id="1460c-p103">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="1460c-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1460c-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1460c-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1460c-122">Request</span></span>
<span data-ttu-id="1460c-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1460c-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="1460c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="1460c-124">Response</span></span>
<span data-ttu-id="1460c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1460c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Fanny Downs",
        "address": "fannyd@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->