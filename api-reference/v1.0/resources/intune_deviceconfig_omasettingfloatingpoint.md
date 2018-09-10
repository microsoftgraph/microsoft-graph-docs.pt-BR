# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="4c3b5-101">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="4c3b5-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="4c3b5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c3b5-103">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="4c3b5-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c3b5-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c3b5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c3b5-105">Properties</span></span>
|<span data-ttu-id="4c3b5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c3b5-106">Property</span></span>|<span data-ttu-id="4c3b5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c3b5-107">Type</span></span>|<span data-ttu-id="4c3b5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c3b5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c3b5-109">displayName</span><span class="sxs-lookup"><span data-stu-id="4c3b5-109">displayName</span></span>|<span data-ttu-id="4c3b5-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c3b5-110">String</span></span>|<span data-ttu-id="4c3b5-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-111">Display Name.</span></span> <span data-ttu-id="4c3b5-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c3b5-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4c3b5-113">descrição</span><span class="sxs-lookup"><span data-stu-id="4c3b5-113">description</span></span>|<span data-ttu-id="4c3b5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c3b5-114">String</span></span>|<span data-ttu-id="4c3b5-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-115">Description.</span></span> <span data-ttu-id="4c3b5-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c3b5-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4c3b5-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="4c3b5-117">omaUri</span></span>|<span data-ttu-id="4c3b5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c3b5-118">String</span></span>|<span data-ttu-id="4c3b5-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-119">OMA.</span></span> <span data-ttu-id="4c3b5-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c3b5-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="4c3b5-121">value</span><span class="sxs-lookup"><span data-stu-id="4c3b5-121">value</span></span>|<span data-ttu-id="4c3b5-122">Single</span><span class="sxs-lookup"><span data-stu-id="4c3b5-122">Single</span></span>|<span data-ttu-id="4c3b5-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c3b5-124">Relações</span><span class="sxs-lookup"><span data-stu-id="4c3b5-124">Relationships</span></span>
<span data-ttu-id="4c3b5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c3b5-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c3b5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c3b5-126">JSON Representation</span></span>
<span data-ttu-id="4c3b5-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c3b5-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```








