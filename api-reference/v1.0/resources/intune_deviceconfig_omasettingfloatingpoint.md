# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="df93d-101">Tipo de recurso omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="df93d-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="df93d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df93d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df93d-103">Definição de ponto flutuante para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="df93d-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="df93d-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df93d-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df93d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df93d-105">Properties</span></span>
|<span data-ttu-id="df93d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df93d-106">Property</span></span>|<span data-ttu-id="df93d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="df93d-107">Type</span></span>|<span data-ttu-id="df93d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="df93d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df93d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="df93d-109">displayName</span></span>|<span data-ttu-id="df93d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df93d-110">String</span></span>|<span data-ttu-id="df93d-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="df93d-111">Display Name</span></span> <span data-ttu-id="df93d-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df93d-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="df93d-113">descrição</span><span class="sxs-lookup"><span data-stu-id="df93d-113">description</span></span>|<span data-ttu-id="df93d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df93d-114">String</span></span>|<span data-ttu-id="df93d-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="df93d-115">Description.</span></span> <span data-ttu-id="df93d-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df93d-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="df93d-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="df93d-117">omaUri</span></span>|<span data-ttu-id="df93d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df93d-118">String</span></span>|<span data-ttu-id="df93d-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="df93d-119">OMA.</span></span> <span data-ttu-id="df93d-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="df93d-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="df93d-121">value</span><span class="sxs-lookup"><span data-stu-id="df93d-121">value</span></span>|<span data-ttu-id="df93d-122">Single</span><span class="sxs-lookup"><span data-stu-id="df93d-122">Single</span></span>|<span data-ttu-id="df93d-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="df93d-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df93d-124">Relações</span><span class="sxs-lookup"><span data-stu-id="df93d-124">Relationships</span></span>
<span data-ttu-id="df93d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df93d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df93d-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df93d-126">JSON Representation</span></span>
<span data-ttu-id="df93d-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df93d-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



