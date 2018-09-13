# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="6d8a1-101">tipo de recurso fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="6d8a1-101">fileSecurityState resource type</span></span>

<span data-ttu-id="6d8a1-102">Contém informações sobre o arquivo (não processo) relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="6d8a1-102">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="6d8a1-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d8a1-103">Properties</span></span>

| <span data-ttu-id="6d8a1-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d8a1-104">Property</span></span>   | <span data-ttu-id="6d8a1-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d8a1-105">Type</span></span>|<span data-ttu-id="6d8a1-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d8a1-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d8a1-107">fileHash</span><span class="sxs-lookup"><span data-stu-id="6d8a1-107">fileHash</span></span>|[<span data-ttu-id="6d8a1-108">fileHash</span><span class="sxs-lookup"><span data-stu-id="6d8a1-108">fileHash</span></span>](filehash.md)|<span data-ttu-id="6d8a1-109">Tipo complexo contendo hashes de arquivo (criptográficos e sensíveis à localização).</span><span class="sxs-lookup"><span data-stu-id="6d8a1-109">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="6d8a1-110">name</span><span class="sxs-lookup"><span data-stu-id="6d8a1-110">name</span></span>|<span data-ttu-id="6d8a1-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d8a1-111">String</span></span>|<span data-ttu-id="6d8a1-112">Nome do arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="6d8a1-112">File name (without path).</span></span>|
|<span data-ttu-id="6d8a1-113">path</span><span class="sxs-lookup"><span data-stu-id="6d8a1-113">path</span></span>|<span data-ttu-id="6d8a1-114">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d8a1-114">String</span></span>|<span data-ttu-id="6d8a1-115">Caminho completo do arquivo/arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="6d8a1-115">Full file path of the stencil file</span></span>|
|<span data-ttu-id="6d8a1-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="6d8a1-116">riskScore</span></span>|<span data-ttu-id="6d8a1-117">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d8a1-117">String</span></span>|<span data-ttu-id="6d8a1-118">Classificação de risco do arquivo de alerta gerada/calculada pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="6d8a1-118">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="6d8a1-119">Intervalo de valor recomendado de 0-1, que equivale a um percentual.</span><span class="sxs-lookup"><span data-stu-id="6d8a1-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d8a1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d8a1-120">JSON representation</span></span>

<span data-ttu-id="6d8a1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d8a1-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->