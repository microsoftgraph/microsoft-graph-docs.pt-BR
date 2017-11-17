# <a name="create-sectiongroup"></a><span data-ttu-id="46a00-101">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="46a00-101">Create sectionGroup</span></span>

<span data-ttu-id="46a00-102">Crie um novo [grupo de seção](../resources/sectiongroup.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="46a00-102">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="46a00-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="46a00-103">Permissions</span></span>
<span data-ttu-id="46a00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="46a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="46a00-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46a00-106">Permission type</span></span>      | <span data-ttu-id="46a00-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46a00-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46a00-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46a00-108">Delegated (work or school account)</span></span> | <span data-ttu-id="46a00-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a00-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="46a00-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46a00-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a00-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a00-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="46a00-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46a00-112">Application</span></span> | <span data-ttu-id="46a00-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a00-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46a00-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46a00-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="46a00-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46a00-115">Request headers</span></span>
| <span data-ttu-id="46a00-116">Nome</span><span class="sxs-lookup"><span data-stu-id="46a00-116">Name</span></span>       | <span data-ttu-id="46a00-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="46a00-117">Type</span></span> | <span data-ttu-id="46a00-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a00-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46a00-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="46a00-119">Authorization</span></span>  | <span data-ttu-id="46a00-120">string</span><span class="sxs-lookup"><span data-stu-id="46a00-120">string</span></span>  | <span data-ttu-id="46a00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46a00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46a00-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46a00-123">Content-Type</span></span> | <span data-ttu-id="46a00-124">string</span><span class="sxs-lookup"><span data-stu-id="46a00-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="46a00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46a00-125">Request body</span></span>
<span data-ttu-id="46a00-126">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="46a00-126">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="46a00-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="46a00-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="46a00-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a00-129">Response</span></span>

<span data-ttu-id="46a00-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46a00-130">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46a00-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46a00-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46a00-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46a00-132">Request</span></span>
<span data-ttu-id="46a00-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46a00-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="46a00-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46a00-134">Response</span></span>
<span data-ttu-id="46a00-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46a00-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
