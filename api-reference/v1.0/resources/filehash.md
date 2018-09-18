# <a name="filehash-resource-type"></a><span data-ttu-id="1d047-101">Tipo de recurso fileHash</span><span class="sxs-lookup"><span data-stu-id="1d047-101">fileHash resource type</span></span>

<span data-ttu-id="1d047-102">Contém informações com estado sobre hashes de arquivo (criptográficos e com localização confidencial).</span><span class="sxs-lookup"><span data-stu-id="1d047-102">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="1d047-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d047-103">Properties</span></span>

| <span data-ttu-id="1d047-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d047-104">Property</span></span>     | <span data-ttu-id="1d047-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d047-105">Type</span></span>        | <span data-ttu-id="1d047-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d047-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d047-107">hashType</span><span class="sxs-lookup"><span data-stu-id="1d047-107">hashType</span></span>|<span data-ttu-id="1d047-108">fileHashType</span><span class="sxs-lookup"><span data-stu-id="1d047-108">fileHashType</span></span>|<span data-ttu-id="1d047-109">Tipo de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d047-109">File hash type.</span></span> <span data-ttu-id="1d047-110">Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="1d047-110">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="1d047-111">hashValue</span><span class="sxs-lookup"><span data-stu-id="1d047-111">hashValue</span></span>|<span data-ttu-id="1d047-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d047-112">String</span></span>|<span data-ttu-id="1d047-113">Valor de hash do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d047-113">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d047-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d047-114">JSON representation</span></span>

<span data-ttu-id="1d047-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d047-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->