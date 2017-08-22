# <a name="create-sectiongroup"></a><span data-ttu-id="88548-101">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="88548-101">Create sectionGroup</span></span>

<span data-ttu-id="88548-102">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="88548-102">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88548-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88548-103">Prerequisites</span></span>
<span data-ttu-id="88548-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="88548-104">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="88548-105">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88548-105">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="88548-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88548-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="88548-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88548-107">Request headers</span></span>
| <span data-ttu-id="88548-108">Nome</span><span class="sxs-lookup"><span data-stu-id="88548-108">Name</span></span>       | <span data-ttu-id="88548-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="88548-109">Type</span></span> | <span data-ttu-id="88548-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88548-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88548-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="88548-111">Authorization</span></span>  | <span data-ttu-id="88548-112">string</span><span class="sxs-lookup"><span data-stu-id="88548-112">string</span></span>  | <span data-ttu-id="88548-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88548-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88548-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88548-115">Content-Type</span></span> | <span data-ttu-id="88548-116">string</span><span class="sxs-lookup"><span data-stu-id="88548-116">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="88548-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88548-117">Request body</span></span>
<span data-ttu-id="88548-118">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="88548-118">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="88548-p102">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="88548-p102">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="88548-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="88548-121">Response</span></span>

<span data-ttu-id="88548-122">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88548-122">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88548-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88548-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88548-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88548-124">Request</span></span>
<span data-ttu-id="88548-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88548-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="88548-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="88548-126">Response</span></span>
<span data-ttu-id="88548-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88548-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedBy": 
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