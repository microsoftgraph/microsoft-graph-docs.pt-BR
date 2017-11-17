# <a name="list-overrides"></a><span data-ttu-id="205b5-101">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="205b5-101">List overrides</span></span>

<span data-ttu-id="205b5-102">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="205b5-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="205b5-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="205b5-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="205b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="205b5-105">Permissions</span></span>
<span data-ttu-id="205b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="205b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="205b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="205b5-108">Permission type</span></span>      | <span data-ttu-id="205b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="205b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="205b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="205b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="205b5-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="205b5-111">Mail.Read</span></span>    |
|<span data-ttu-id="205b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="205b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="205b5-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="205b5-113">Mail.Read</span></span>    |
|<span data-ttu-id="205b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="205b5-114">Application</span></span> | <span data-ttu-id="205b5-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="205b5-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="205b5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="205b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="205b5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="205b5-117">Request headers</span></span>
| <span data-ttu-id="205b5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="205b5-118">Name</span></span>       | <span data-ttu-id="205b5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="205b5-119">Type</span></span> | <span data-ttu-id="205b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="205b5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="205b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="205b5-121">Authorization</span></span>  | <span data-ttu-id="205b5-122">string</span><span class="sxs-lookup"><span data-stu-id="205b5-122">string</span></span>  | <span data-ttu-id="205b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="205b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="205b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="205b5-125">Request body</span></span>
<span data-ttu-id="205b5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="205b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="205b5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="205b5-127">Response</span></span>

<span data-ttu-id="205b5-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta. Retorna uma coleção vazia se o usuário não tiver quaisquer substituições configuradas.</span><span class="sxs-lookup"><span data-stu-id="205b5-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="205b5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="205b5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="205b5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="205b5-131">Request</span></span>
<span data-ttu-id="205b5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="205b5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="205b5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="205b5-133">Response</span></span>
<span data-ttu-id="205b5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="205b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
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