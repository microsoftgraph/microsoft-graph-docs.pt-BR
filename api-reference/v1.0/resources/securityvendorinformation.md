# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="15e80-101">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="15e80-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="15e80-102">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="15e80-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="15e80-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15e80-103">Properties</span></span>

| <span data-ttu-id="15e80-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15e80-104">Property</span></span>   | <span data-ttu-id="15e80-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="15e80-105">Type</span></span>|<span data-ttu-id="15e80-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="15e80-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15e80-107">provedor</span><span class="sxs-lookup"><span data-stu-id="15e80-107">provider</span></span> |<span data-ttu-id="15e80-108">String</span><span class="sxs-lookup"><span data-stu-id="15e80-108">String</span></span>|<span data-ttu-id="15e80-109">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="15e80-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="15e80-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="15e80-110">providerVersion</span></span>|<span data-ttu-id="15e80-111">String</span><span class="sxs-lookup"><span data-stu-id="15e80-111">String</span></span>|<span data-ttu-id="15e80-112">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="15e80-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="15e80-113">*Required*</span><span class="sxs-lookup"><span data-stu-id="15e80-113">*Required*</span></span>|
|<span data-ttu-id="15e80-114">subProvider</span><span class="sxs-lookup"><span data-stu-id="15e80-114">subProvider</span></span>|<span data-ttu-id="15e80-115">String</span><span class="sxs-lookup"><span data-stu-id="15e80-115">String</span></span>|<span data-ttu-id="15e80-116">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="15e80-116">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="15e80-117">fornecedor</span><span class="sxs-lookup"><span data-stu-id="15e80-117">vendor</span></span> |<span data-ttu-id="15e80-118">String</span><span class="sxs-lookup"><span data-stu-id="15e80-118">String</span></span>|<span data-ttu-id="15e80-119">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="15e80-119">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="15e80-120">*Required*</span><span class="sxs-lookup"><span data-stu-id="15e80-120">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="15e80-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15e80-121">JSON representation</span></span>

<span data-ttu-id="15e80-122">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15e80-122">The folllowing is a JSON representation of the resource.</span></span>
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
