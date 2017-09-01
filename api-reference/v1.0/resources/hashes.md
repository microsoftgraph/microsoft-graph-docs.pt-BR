# <a name="hashes-resource-type"></a><span data-ttu-id="01720-101">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="01720-101">Hashes resource type</span></span>

<span data-ttu-id="01720-102">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="01720-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="01720-103">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="01720-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01720-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01720-104">JSON representation</span></span>

<span data-ttu-id="01720-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01720-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a><span data-ttu-id="01720-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01720-106">Properties</span></span>

| <span data-ttu-id="01720-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01720-107">Property</span></span>         | <span data-ttu-id="01720-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="01720-108">Type</span></span>   | <span data-ttu-id="01720-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="01720-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="01720-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="01720-110">**sha1Hash**</span></span>     | <span data-ttu-id="01720-111">String</span><span class="sxs-lookup"><span data-stu-id="01720-111">String</span></span> | <span data-ttu-id="01720-p101">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01720-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="01720-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="01720-114">**crc32Hash**</span></span>    | <span data-ttu-id="01720-115">String</span><span class="sxs-lookup"><span data-stu-id="01720-115">String</span></span> | <span data-ttu-id="01720-p102">O valor de CRC32 do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01720-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="01720-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="01720-118">**quickXorHash**</span></span> | <span data-ttu-id="01720-119">String</span><span class="sxs-lookup"><span data-stu-id="01720-119">String</span></span> | <span data-ttu-id="01720-p103">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01720-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="01720-p104">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="01720-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>


## <a name="remarks"></a><span data-ttu-id="01720-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="01720-124">Remarks</span></span>

<span data-ttu-id="01720-p105">No OneDrive for Business, **sha1Hash** e **crc32Hash** não estão disponíveis. No OneDrive Personal, **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="01720-p105">In OneDrive for Business, **sha1Hash** and **crc32Hash** are not available. In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="01720-127">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="01720-127">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
