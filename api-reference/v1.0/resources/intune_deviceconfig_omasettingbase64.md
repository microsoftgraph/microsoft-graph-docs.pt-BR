# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="6dda1-101">Tipo de recurso omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="6dda1-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="6dda1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6dda1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dda1-103">Definição de Base64 das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="6dda1-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="6dda1-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6dda1-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6dda1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dda1-105">Properties</span></span>
|<span data-ttu-id="6dda1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dda1-106">Property</span></span>|<span data-ttu-id="6dda1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dda1-107">Type</span></span>|<span data-ttu-id="6dda1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dda1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dda1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6dda1-109">displayName</span></span>|<span data-ttu-id="6dda1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dda1-110">String</span></span>|<span data-ttu-id="6dda1-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6dda1-111">Display Name.</span></span> <span data-ttu-id="6dda1-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6dda1-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6dda1-113">descrição</span><span class="sxs-lookup"><span data-stu-id="6dda1-113">description</span></span>|<span data-ttu-id="6dda1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dda1-114">String</span></span>|<span data-ttu-id="6dda1-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="6dda1-115">Description.</span></span> <span data-ttu-id="6dda1-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6dda1-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6dda1-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="6dda1-117">omaUri</span></span>|<span data-ttu-id="6dda1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dda1-118">String</span></span>|<span data-ttu-id="6dda1-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="6dda1-119">OMA.</span></span> <span data-ttu-id="6dda1-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6dda1-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="6dda1-121">fileName</span><span class="sxs-lookup"><span data-stu-id="6dda1-121">fileName</span></span>|<span data-ttu-id="6dda1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dda1-122">String</span></span>|<span data-ttu-id="6dda1-123">Nome de arquivo associado com a propriedade do valor (\*.cer</span><span class="sxs-lookup"><span data-stu-id="6dda1-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="6dda1-124">\*.crt ).</span><span class="sxs-lookup"><span data-stu-id="6dda1-124">\*.crt ).</span></span>|
|<span data-ttu-id="6dda1-125">valor</span><span class="sxs-lookup"><span data-stu-id="6dda1-125">value</span></span>|<span data-ttu-id="6dda1-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dda1-126">String</span></span>|<span data-ttu-id="6dda1-127">Valor.</span><span class="sxs-lookup"><span data-stu-id="6dda1-127">Value.</span></span> <span data-ttu-id="6dda1-128">(Cadeia de caracteres codificada em Base64)</span><span class="sxs-lookup"><span data-stu-id="6dda1-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dda1-129">Relações</span><span class="sxs-lookup"><span data-stu-id="6dda1-129">Relationships</span></span>
<span data-ttu-id="6dda1-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dda1-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6dda1-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dda1-131">JSON Representation</span></span>
<span data-ttu-id="6dda1-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dda1-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



