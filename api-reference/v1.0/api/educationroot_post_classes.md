# <a name="create-educationclass"></a><span data-ttu-id="1d417-101">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="1d417-101">Create educationClass</span></span>

<span data-ttu-id="1d417-102">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="1d417-102">Create a new class.</span></span> <span data-ttu-id="1d417-103">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="1d417-103">This will also create a universal group.</span></span> <span data-ttu-id="1d417-104">Quando você usar essa API para criar uma aula, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1d417-104">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d417-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d417-105">Permissions</span></span>
<span data-ttu-id="1d417-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d417-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d417-108">Permission type</span></span>      | <span data-ttu-id="1d417-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d417-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d417-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d417-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1d417-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d417-111">Not supported.</span></span>  |
|<span data-ttu-id="1d417-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d417-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1d417-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d417-113">Not supported.</span></span>  |
|<span data-ttu-id="1d417-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d417-114">Application</span></span> | <span data-ttu-id="1d417-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d417-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1d417-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d417-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="1d417-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d417-117">Request headers</span></span>
| <span data-ttu-id="1d417-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d417-118">Header</span></span>       | <span data-ttu-id="1d417-119">Valor</span><span class="sxs-lookup"><span data-stu-id="1d417-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d417-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d417-120">Authorization</span></span>  | <span data-ttu-id="1d417-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d417-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d417-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d417-123">Content-Type</span></span>  | <span data-ttu-id="1d417-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d417-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d417-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d417-125">Request body</span></span>
<span data-ttu-id="1d417-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="1d417-126">In the request body, supply a JSON representation of an [invitation](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="1d417-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d417-127">Response</span></span>
<span data-ttu-id="1d417-128">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d417-128">If successful, this method returns a `201 Created` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d417-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d417-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d417-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d417-130">Request</span></span>
<span data-ttu-id="1d417-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d417-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="1d417-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d417-132">Response</span></span>
<span data-ttu-id="1d417-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d417-133">The following is an example of the response.</span></span> 

><span data-ttu-id="1d417-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d417-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->