# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="ecd3c-101">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="ecd3c-101">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="ecd3c-102">Obtenha a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-102">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="ecd3c-103">Ao configurar um cliente do Outlook, o usuário seleciona o idioma de preferência na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-103">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="ecd3c-104">Posteriormente, é possível obter o idioma de sua preferência [acessando as configurações da caixa de correio do usuário](user_get_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ecd3c-104">You can subsequently get the preferred language by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="ecd3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecd3c-105">Permissions</span></span>
<span data-ttu-id="ecd3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ecd3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ecd3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecd3c-108">Permission type</span></span>      | <span data-ttu-id="ecd3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecd3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecd3c-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecd3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ecd3c-111">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ecd3c-111">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="ecd3c-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecd3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecd3c-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="ecd3c-113">User.Read</span></span>    |
|<span data-ttu-id="ecd3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecd3c-114">Application</span></span> | <span data-ttu-id="ecd3c-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecd3c-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecd3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecd3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="ecd3c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3c-117">Request headers</span></span>
| <span data-ttu-id="ecd3c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ecd3c-118">Name</span></span>       | <span data-ttu-id="ecd3c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecd3c-119">Type</span></span> | <span data-ttu-id="ecd3c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd3c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ecd3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecd3c-121">Authorization</span></span>  | <span data-ttu-id="ecd3c-122">string</span><span class="sxs-lookup"><span data-stu-id="ecd3c-122">string</span></span>  | <span data-ttu-id="ecd3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ecd3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3c-125">Request body</span></span>
<span data-ttu-id="ecd3c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecd3c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd3c-127">Response</span></span>
<span data-ttu-id="ecd3c-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localeInfo](../resources/localeinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecd3c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecd3c-129">Example</span></span>
<span data-ttu-id="ecd3c-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ecd3c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3c-131">Request</span></span>
<span data-ttu-id="ecd3c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="ecd3c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd3c-133">Response</span></span>
<span data-ttu-id="ecd3c-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecd3c-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->