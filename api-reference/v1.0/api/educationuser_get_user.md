# <a name="get-user"></a><span data-ttu-id="bbef1-101">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="bbef1-101">Get user</span></span>

<span data-ttu-id="bbef1-102">Recupere o **usuário** do diretório simples que corresponde a esse **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="bbef1-102">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="bbef1-103">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="bbef1-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="bbef1-104">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="bbef1-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbef1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbef1-105">Permissions</span></span>
<span data-ttu-id="bbef1-106">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bbef1-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="bbef1-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bbef1-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bbef1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbef1-108">Permission type</span></span>      | <span data-ttu-id="bbef1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbef1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbef1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbef1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bbef1-111">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbef1-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="bbef1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbef1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bbef1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbef1-113">Not supported.</span></span>  |
|<span data-ttu-id="bbef1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbef1-114">Application</span></span> | <span data-ttu-id="bbef1-115">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbef1-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="bbef1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbef1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="bbef1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbef1-117">Request headers</span></span>
| <span data-ttu-id="bbef1-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbef1-118">Header</span></span>       | <span data-ttu-id="bbef1-119">Valor</span><span class="sxs-lookup"><span data-stu-id="bbef1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbef1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbef1-120">Authorization</span></span>  | <span data-ttu-id="bbef1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbef1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbef1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbef1-123">Request body</span></span>
<span data-ttu-id="bbef1-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbef1-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bbef1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbef1-125">Response</span></span>
<span data-ttu-id="bbef1-126">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbef1-126">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbef1-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbef1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbef1-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbef1-128">Request</span></span>
<span data-ttu-id="bbef1-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbef1-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
##### <a name="response"></a><span data-ttu-id="bbef1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbef1-130">Response</span></span>
<span data-ttu-id="bbef1-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbef1-131">The following is an example of the response.</span></span> 

><span data-ttu-id="bbef1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbef1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->