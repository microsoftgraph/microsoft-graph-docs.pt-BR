# <a name="get-educationclass"></a><span data-ttu-id="eac8c-101">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="eac8c-101">Get educationClass</span></span>

<span data-ttu-id="eac8c-102">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="eac8c-102">Retrieve a class from the system.</span></span> <span data-ttu-id="eac8c-103">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="eac8c-103">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="eac8c-104">Os membros do grupo representam os alunos; os administradores do grupo representam os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="eac8c-104">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="eac8c-105">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="eac8c-105">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="eac8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac8c-106">Permissions</span></span>
<span data-ttu-id="eac8c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eac8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eac8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eac8c-109">Permission type</span></span>      | <span data-ttu-id="eac8c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eac8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eac8c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eac8c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="eac8c-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="eac8c-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="eac8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eac8c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eac8c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eac8c-114">Not supported</span></span>  |
|<span data-ttu-id="eac8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eac8c-115">Application</span></span> | <span data-ttu-id="eac8c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac8c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eac8c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eac8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eac8c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eac8c-118">Optional query parameters</span></span>
<span data-ttu-id="eac8c-119">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eac8c-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eac8c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eac8c-120">Request headers</span></span>
| <span data-ttu-id="eac8c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eac8c-121">Header</span></span>       | <span data-ttu-id="eac8c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eac8c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eac8c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eac8c-123">Authorization</span></span>  | <span data-ttu-id="eac8c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac8c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eac8c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eac8c-126">Request body</span></span>
<span data-ttu-id="eac8c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eac8c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eac8c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac8c-128">Response</span></span>
<span data-ttu-id="eac8c-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eac8c-129">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eac8c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eac8c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eac8c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac8c-131">Request</span></span>
<span data-ttu-id="eac8c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac8c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="eac8c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac8c-133">Response</span></span>
<span data-ttu-id="eac8c-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eac8c-134">The following is an example of the response.</span></span> 

><span data-ttu-id="eac8c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eac8c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->