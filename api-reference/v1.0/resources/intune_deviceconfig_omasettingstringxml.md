# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="14526-101">Tipo de recurso omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="14526-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="14526-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="14526-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14526-103">Definição de StringXML para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="14526-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="14526-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="14526-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14526-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14526-105">Properties</span></span>
|<span data-ttu-id="14526-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14526-106">Property</span></span>|<span data-ttu-id="14526-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="14526-107">Type</span></span>|<span data-ttu-id="14526-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="14526-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14526-109">displayName</span><span class="sxs-lookup"><span data-stu-id="14526-109">displayName</span></span>|<span data-ttu-id="14526-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14526-110">String</span></span>|<span data-ttu-id="14526-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="14526-111">Display Name</span></span> <span data-ttu-id="14526-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="14526-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="14526-113">descrição</span><span class="sxs-lookup"><span data-stu-id="14526-113">description</span></span>|<span data-ttu-id="14526-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14526-114">String</span></span>|<span data-ttu-id="14526-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="14526-115">Description.</span></span> <span data-ttu-id="14526-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="14526-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="14526-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="14526-117">omaUri</span></span>|<span data-ttu-id="14526-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14526-118">String</span></span>|<span data-ttu-id="14526-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="14526-119">OMA.</span></span> <span data-ttu-id="14526-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="14526-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="14526-121">fileName</span><span class="sxs-lookup"><span data-stu-id="14526-121">fileName</span></span>|<span data-ttu-id="14526-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14526-122">String</span></span>|<span data-ttu-id="14526-123">Nome do arquivo associado à propriedade de valor (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="14526-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="14526-124">valor</span><span class="sxs-lookup"><span data-stu-id="14526-124">value</span></span>|<span data-ttu-id="14526-125">Binário</span><span class="sxs-lookup"><span data-stu-id="14526-125">Binary</span></span>|<span data-ttu-id="14526-126">Valor.</span><span class="sxs-lookup"><span data-stu-id="14526-126">Value.</span></span> <span data-ttu-id="14526-127">(Matriz de bytes codificados de UTF8)</span><span class="sxs-lookup"><span data-stu-id="14526-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="14526-128">Relações</span><span class="sxs-lookup"><span data-stu-id="14526-128">Relationships</span></span>
<span data-ttu-id="14526-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14526-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14526-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14526-130">JSON Representation</span></span>
<span data-ttu-id="14526-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14526-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



