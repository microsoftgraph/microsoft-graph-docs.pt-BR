# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="6427d-101">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="6427d-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="6427d-102">Contém detalhes sobre o fornecedor, provedor e subprovedor de produtos/serviços de segurança (por exemplo,  vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="6427d-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="6427d-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6427d-103">Properties</span></span>

| <span data-ttu-id="6427d-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6427d-104">Property</span></span>   | <span data-ttu-id="6427d-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6427d-105">Type</span></span>|<span data-ttu-id="6427d-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6427d-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6427d-107">provider \*</span><span class="sxs-lookup"><span data-stu-id="6427d-107">provider \*</span></span>|<span data-ttu-id="6427d-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6427d-108">String</span></span>|<span data-ttu-id="6427d-109">Provedor específico (produto/serviço - não a empresa fornecedora); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="6427d-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="6427d-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="6427d-110">providerVersion</span></span>|<span data-ttu-id="6427d-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6427d-111">String</span></span>|<span data-ttu-id="6427d-112">Versão do provedor ou subprovidor, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="6427d-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span>|
|<span data-ttu-id="6427d-113">subProvider</span><span class="sxs-lookup"><span data-stu-id="6427d-113">subProvider</span></span>|<span data-ttu-id="6427d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6427d-114">String</span></span>|<span data-ttu-id="6427d-115">Subprovidor específico (sob o provedor agregador); por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="6427d-115">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="6427d-116">vendor \*</span><span class="sxs-lookup"><span data-stu-id="6427d-116">vendor \*</span></span>|<span data-ttu-id="6427d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6427d-117">String</span></span>|<span data-ttu-id="6427d-118">Nome do fornecedor de alertas (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="6427d-118">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span>|
<span data-ttu-id="6427d-119">(\* Indica um campo obrigatório.)</span><span class="sxs-lookup"><span data-stu-id="6427d-119">(\* Indicates a mandatory field.)</span></span>

## <a name="json-representation"></a><span data-ttu-id="6427d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6427d-120">JSON representation</span></span>

<span data-ttu-id="6427d-121">A seguir, uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6427d-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
