# <a name="educationstudent-resource-type"></a><span data-ttu-id="58424-101">Tipo de recurso educationStudent</span><span class="sxs-lookup"><span data-stu-id="58424-101">educationStudent resource type</span></span>

<span data-ttu-id="58424-102">Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.</span><span class="sxs-lookup"><span data-stu-id="58424-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="58424-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58424-103">Properties</span></span>
| <span data-ttu-id="58424-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58424-104">Property</span></span>     | <span data-ttu-id="58424-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="58424-105">Type</span></span>   |<span data-ttu-id="58424-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="58424-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58424-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="58424-107">birthDate</span></span>|<span data-ttu-id="58424-108">Data</span><span class="sxs-lookup"><span data-stu-id="58424-108">Date</span></span>| <span data-ttu-id="58424-109">Data de nascimento do aluno.</span><span class="sxs-lookup"><span data-stu-id="58424-109">Birth date of the student.</span></span>|
|<span data-ttu-id="58424-110">externalId</span><span class="sxs-lookup"><span data-stu-id="58424-110">externalId</span></span>|<span data-ttu-id="58424-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58424-111">String</span></span>| <span data-ttu-id="58424-112">ID do aluno no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="58424-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="58424-113">gender</span><span class="sxs-lookup"><span data-stu-id="58424-113">gender</span></span>|<span data-ttu-id="58424-114">educationGender</span><span class="sxs-lookup"><span data-stu-id="58424-114">educationGender values</span></span>| <span data-ttu-id="58424-115">Os valores possíveis são: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="58424-115">The possible values are `female`, `male`, `other`, `unknownFutureValue`, , , , , , , , or .</span></span>|
|<span data-ttu-id="58424-116">grade</span><span class="sxs-lookup"><span data-stu-id="58424-116">grade</span></span>|<span data-ttu-id="58424-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58424-117">String</span></span>|<span data-ttu-id="58424-118">Nível de classificação atual do aluno.</span><span class="sxs-lookup"><span data-stu-id="58424-118">Current grade level of the student.</span></span>|
|<span data-ttu-id="58424-119">graduationYear</span><span class="sxs-lookup"><span data-stu-id="58424-119">graduationYear</span></span>|<span data-ttu-id="58424-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58424-120">String</span></span>| <span data-ttu-id="58424-121">Ano que o aluno está graduando na escola.</span><span class="sxs-lookup"><span data-stu-id="58424-121">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="58424-122">studentNumber</span><span class="sxs-lookup"><span data-stu-id="58424-122">studentNumber</span></span>|<span data-ttu-id="58424-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58424-123">String</span></span>| <span data-ttu-id="58424-124">Número do aluno.</span><span class="sxs-lookup"><span data-stu-id="58424-124">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58424-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58424-125">JSON representation</span></span>

<span data-ttu-id="58424-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58424-126">The following is a JSON representation of the resource.</span></span>

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
