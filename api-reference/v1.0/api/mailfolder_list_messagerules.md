# <a name="list-rules"></a><span data-ttu-id="0a65e-101">Listar regras</span><span class="sxs-lookup"><span data-stu-id="0a65e-101">List rules</span></span>

<span data-ttu-id="0a65e-102">Obtenha todos os objetos [messageRule](../resources/messagerule.md) definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a65e-102">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a65e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a65e-103">Permissions</span></span>
<span data-ttu-id="0a65e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a65e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a65e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a65e-106">Permission type</span></span>      | <span data-ttu-id="0a65e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a65e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a65e-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a65e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0a65e-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0a65e-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0a65e-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a65e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a65e-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0a65e-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0a65e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a65e-112">Application</span></span> | <span data-ttu-id="0a65e-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0a65e-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a65e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a65e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a65e-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a65e-115">Optional query parameters</span></span>
<span data-ttu-id="0a65e-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a65e-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0a65e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a65e-117">Request headers</span></span>
| <span data-ttu-id="0a65e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0a65e-118">Name</span></span>       | <span data-ttu-id="0a65e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a65e-119">Type</span></span> | <span data-ttu-id="0a65e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a65e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a65e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a65e-121">Authorization</span></span>  | <span data-ttu-id="0a65e-122">string</span><span class="sxs-lookup"><span data-stu-id="0a65e-122">string</span></span>  | <span data-ttu-id="0a65e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a65e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a65e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a65e-125">Request body</span></span>
<span data-ttu-id="0a65e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a65e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0a65e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a65e-127">Response</span></span>
<span data-ttu-id="0a65e-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a65e-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a65e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a65e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a65e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a65e-130">Request</span></span>
<span data-ttu-id="0a65e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a65e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="0a65e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a65e-132">Response</span></span>
<span data-ttu-id="0a65e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a65e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
      "id":"AQAAAJ5dZqA=",
      "displayName":"From partner",
      "sequence":2,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "senderContains":[
          "ADELE"
        ]
      },
      "actions":{
        "stopProcessingRules":true,
        "forwardTo":[
          {
            "emailAddress":{
              "name":"Alex Wilbur",
              "address":"AlexW@contoso.onmicrosoft.com"
            }
          }
        ]
      }
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
