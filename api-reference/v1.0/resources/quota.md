# <a name="quota-resource-type"></a><span data-ttu-id="d88f0-101">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="d88f0-101">Quota resource type</span></span>

<span data-ttu-id="d88f0-102">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="d88f0-102">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d88f0-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d88f0-103">JSON representation</span></span>

<span data-ttu-id="d88f0-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d88f0-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="d88f0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d88f0-105">Properties</span></span>

| <span data-ttu-id="d88f0-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d88f0-106">Property name</span></span> | <span data-ttu-id="d88f0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d88f0-107">Type</span></span>   | <span data-ttu-id="d88f0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88f0-108">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="d88f0-109">total</span><span class="sxs-lookup"><span data-stu-id="d88f0-109">total</span></span>         | <span data-ttu-id="d88f0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d88f0-110">Int64</span></span>  | <span data-ttu-id="d88f0-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="d88f0-113">used</span><span class="sxs-lookup"><span data-stu-id="d88f0-113">used</span></span>          | <span data-ttu-id="d88f0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d88f0-114">Int64</span></span>  | <span data-ttu-id="d88f0-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="d88f0-117">remaining</span><span class="sxs-lookup"><span data-stu-id="d88f0-117">remaining</span></span>     | <span data-ttu-id="d88f0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d88f0-118">Int64</span></span>  | <span data-ttu-id="d88f0-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="d88f0-121">deleted</span><span class="sxs-lookup"><span data-stu-id="d88f0-121">deleted</span></span>       | <span data-ttu-id="d88f0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d88f0-122">Int64</span></span>  | <span data-ttu-id="d88f0-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="d88f0-125">estado</span><span class="sxs-lookup"><span data-stu-id="d88f0-125">state</span></span>         | <span data-ttu-id="d88f0-126">string</span><span class="sxs-lookup"><span data-stu-id="d88f0-126">string</span></span> | <span data-ttu-id="d88f0-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="d88f0-129">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="d88f0-129">State Enumeration</span></span>

| <span data-ttu-id="d88f0-130">Valor</span><span class="sxs-lookup"><span data-stu-id="d88f0-130">Value</span></span>      | <span data-ttu-id="d88f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88f0-131">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="d88f0-132">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="d88f0-132">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="d88f0-133">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="d88f0-133">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="d88f0-134">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="d88f0-134">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="d88f0-p106">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="d88f0-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
