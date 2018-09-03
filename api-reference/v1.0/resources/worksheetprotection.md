# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="a0920-101">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="a0920-101">WorksheetProtection resource type</span></span>

<span data-ttu-id="a0920-102">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="a0920-102">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="a0920-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0920-103">Methods</span></span>

| <span data-ttu-id="a0920-104">Método</span><span class="sxs-lookup"><span data-stu-id="a0920-104">Method</span></span>           | <span data-ttu-id="a0920-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0920-105">Return Type</span></span>    |<span data-ttu-id="a0920-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0920-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0920-107">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="a0920-107">Get WorksheetProtection</span></span>](../api/worksheetprotection_get.md) | [<span data-ttu-id="a0920-108">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="a0920-108">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="a0920-109">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="a0920-109">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="a0920-110">Proteger</span><span class="sxs-lookup"><span data-stu-id="a0920-110">Protect</span></span>](../api/worksheetprotection_protect.md)|<span data-ttu-id="a0920-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0920-111">None</span></span>|<span data-ttu-id="a0920-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="a0920-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="a0920-114">Desproteger</span><span class="sxs-lookup"><span data-stu-id="a0920-114">Unprotect</span></span>](../api/worksheetprotection_unprotect.md)|<span data-ttu-id="a0920-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0920-115">None</span></span>|<span data-ttu-id="a0920-116">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="a0920-116">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="a0920-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0920-117">Properties</span></span>
| <span data-ttu-id="a0920-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0920-118">Property</span></span>     | <span data-ttu-id="a0920-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0920-119">Type</span></span>   |<span data-ttu-id="a0920-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0920-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0920-121">opções</span><span class="sxs-lookup"><span data-stu-id="a0920-121">options</span></span>|[<span data-ttu-id="a0920-122">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="a0920-122">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="a0920-p102">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0920-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="a0920-125">protected</span><span class="sxs-lookup"><span data-stu-id="a0920-125">protected</span></span>|<span data-ttu-id="a0920-126">booliano</span><span class="sxs-lookup"><span data-stu-id="a0920-126">boolean</span></span>|<span data-ttu-id="a0920-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0920-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0920-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0920-129">JSON representation</span></span>

<span data-ttu-id="a0920-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0920-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->