# <a name="get-rule"></a><span data-ttu-id="37458-101">Obter regra</span><span class="sxs-lookup"><span data-stu-id="37458-101">Get rule</span></span>


<span data-ttu-id="37458-102">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="37458-102">Get the properties and relationships of a [calendar](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="37458-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="37458-103">Permissions</span></span>
<span data-ttu-id="37458-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37458-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37458-106">Permission type</span></span>      | <span data-ttu-id="37458-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37458-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37458-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37458-108">Delegated (work or school account)</span></span> | <span data-ttu-id="37458-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="37458-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="37458-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37458-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37458-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="37458-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="37458-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37458-112">Application</span></span> | <span data-ttu-id="37458-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="37458-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="37458-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37458-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37458-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37458-115">Optional query parameters</span></span>
<span data-ttu-id="37458-116">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37458-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37458-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37458-117">Request headers</span></span>
| <span data-ttu-id="37458-118">Nome</span><span class="sxs-lookup"><span data-stu-id="37458-118">Name</span></span>      |<span data-ttu-id="37458-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="37458-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37458-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="37458-120">Authorization</span></span>  | <span data-ttu-id="37458-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37458-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="37458-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37458-123">Request body</span></span>
<span data-ttu-id="37458-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37458-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="37458-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="37458-125">Response</span></span>
<span data-ttu-id="37458-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37458-126">If successful, this method returns a `200 OK` response code and a [deviceManagementExchangeConnector](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37458-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37458-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37458-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37458-128">Request</span></span>
<span data-ttu-id="37458-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37458-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="37458-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="37458-130">Response</span></span>
<span data-ttu-id="37458-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37458-131">Here is an example of the response.</span></span> <span data-ttu-id="37458-132">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="37458-132">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="37458-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37458-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->