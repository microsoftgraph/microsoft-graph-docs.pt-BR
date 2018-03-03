# <a name="educationteacher-resource-type"></a><span data-ttu-id="6479a-101">Tipo de recurso educationTeacher</span><span class="sxs-lookup"><span data-stu-id="6479a-101">educationTeacher resource type</span></span>

<span data-ttu-id="6479a-102">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.</span><span class="sxs-lookup"><span data-stu-id="6479a-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="6479a-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6479a-103">Properties</span></span>
| <span data-ttu-id="6479a-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6479a-104">Property</span></span>     | <span data-ttu-id="6479a-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6479a-105">Type</span></span>   |<span data-ttu-id="6479a-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6479a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6479a-107">externalId</span><span class="sxs-lookup"><span data-stu-id="6479a-107">externalId</span></span>|<span data-ttu-id="6479a-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6479a-108">String</span></span>| <span data-ttu-id="6479a-109">ID do professor no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="6479a-109">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="6479a-110">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="6479a-110">teacherNumber</span></span>|<span data-ttu-id="6479a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6479a-111">String</span></span>|<span data-ttu-id="6479a-112">Número do professor.</span><span class="sxs-lookup"><span data-stu-id="6479a-112">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6479a-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6479a-113">JSON representation</span></span>

<span data-ttu-id="6479a-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6479a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->