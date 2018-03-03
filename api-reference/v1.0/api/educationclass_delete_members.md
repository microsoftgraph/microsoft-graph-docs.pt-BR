# <a name="remove-a-student"></a><span data-ttu-id="aa75d-101">Remover um aluno</span><span class="sxs-lookup"><span data-stu-id="aa75d-101">Remove a student</span></span>

<span data-ttu-id="aa75d-102">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="aa75d-102">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="aa75d-103">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="aa75d-103">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="aa75d-104">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="aa75d-104">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="aa75d-105">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass_list_teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="aa75d-105">Get the list of teachers by calling [educationclass_list_teachers](educationclass_list_teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa75d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa75d-106">Permissions</span></span>
<span data-ttu-id="aa75d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa75d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa75d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa75d-109">Permission type</span></span>      | <span data-ttu-id="aa75d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa75d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa75d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa75d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa75d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa75d-112">Not supported.</span></span>  |
|<span data-ttu-id="aa75d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa75d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aa75d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa75d-114">Not supported.</span></span>  |
|<span data-ttu-id="aa75d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa75d-115">Application</span></span> | <span data-ttu-id="aa75d-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa75d-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa75d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa75d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="aa75d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa75d-118">Request headers</span></span>
| <span data-ttu-id="aa75d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa75d-119">Header</span></span>       | <span data-ttu-id="aa75d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aa75d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa75d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa75d-121">Authorization</span></span>  | <span data-ttu-id="aa75d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa75d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa75d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa75d-124">Request body</span></span>
<span data-ttu-id="aa75d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa75d-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="aa75d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa75d-126">Response</span></span>
<span data-ttu-id="aa75d-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="aa75d-127">If successful, this method returns a `204 No Content` response code and an event object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa75d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa75d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa75d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa75d-129">Request</span></span>
<span data-ttu-id="aa75d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa75d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="aa75d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa75d-131">Response</span></span>
<span data-ttu-id="aa75d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa75d-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
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
