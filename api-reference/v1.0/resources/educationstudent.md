# <a name="educationstudent-resource-type"></a><span data-ttu-id="e3709-101">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="e3709-101">educationStudent resource type</span></span>

<span data-ttu-id="e3709-102">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="e3709-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="e3709-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3709-103">Properties</span></span>
| <span data-ttu-id="e3709-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3709-104">Property</span></span>     | <span data-ttu-id="e3709-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3709-105">Type</span></span>   |<span data-ttu-id="e3709-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3709-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3709-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="e3709-107">birthDate</span></span>|<span data-ttu-id="e3709-108">Data</span><span class="sxs-lookup"><span data-stu-id="e3709-108">Date</span></span>| <span data-ttu-id="e3709-109">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="e3709-109">Birth date of the student.</span></span>|
|<span data-ttu-id="e3709-110">externalId</span><span class="sxs-lookup"><span data-stu-id="e3709-110">externalId</span></span>|<span data-ttu-id="e3709-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3709-111">String</span></span>| <span data-ttu-id="e3709-112">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="e3709-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="e3709-113">gender</span><span class="sxs-lookup"><span data-stu-id="e3709-113">Gender</span></span>|`educationGender enumeration`| <span data-ttu-id="e3709-114">Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e3709-114">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="e3709-115">grade</span><span class="sxs-lookup"><span data-stu-id="e3709-115">QuizInfoPage: grade</span></span>|<span data-ttu-id="e3709-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3709-116">String</span></span>|<span data-ttu-id="e3709-117">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="e3709-117">Current grade level of the student.</span></span>|
|<span data-ttu-id="e3709-118">graduationYear</span><span class="sxs-lookup"><span data-stu-id="e3709-118">graduationYear</span></span>|<span data-ttu-id="e3709-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3709-119">String</span></span>| <span data-ttu-id="e3709-120">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="e3709-120">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="e3709-121">studentNumber</span><span class="sxs-lookup"><span data-stu-id="e3709-121">studentNumber</span></span>|<span data-ttu-id="e3709-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3709-122">String</span></span>| <span data-ttu-id="e3709-123">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="e3709-123">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3709-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3709-124">JSON representation</span></span>

<span data-ttu-id="e3709-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3709-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->