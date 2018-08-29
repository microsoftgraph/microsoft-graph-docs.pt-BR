# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="a0eab-101">Tipo de recurso omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="a0eab-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="a0eab-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0eab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0eab-103">Definição de números inteiros das configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a0eab-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="a0eab-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0eab-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0eab-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0eab-105">Properties</span></span>
|<span data-ttu-id="a0eab-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0eab-106">Property</span></span>|<span data-ttu-id="a0eab-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0eab-107">Type</span></span>|<span data-ttu-id="a0eab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0eab-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0eab-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a0eab-109">displayName</span></span>|<span data-ttu-id="a0eab-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0eab-110">String</span></span>|<span data-ttu-id="a0eab-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a0eab-111">Display Name.</span></span> <span data-ttu-id="a0eab-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0eab-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0eab-113">descrição</span><span class="sxs-lookup"><span data-stu-id="a0eab-113">description</span></span>|<span data-ttu-id="a0eab-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0eab-114">String</span></span>|<span data-ttu-id="a0eab-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a0eab-115">Description.</span></span> <span data-ttu-id="a0eab-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0eab-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0eab-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="a0eab-117">omaUri</span></span>|<span data-ttu-id="a0eab-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0eab-118">String</span></span>|<span data-ttu-id="a0eab-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="a0eab-119">OMA.</span></span> <span data-ttu-id="a0eab-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a0eab-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="a0eab-121">valor</span><span class="sxs-lookup"><span data-stu-id="a0eab-121">value</span></span>|<span data-ttu-id="a0eab-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a0eab-122">Int32</span></span>|<span data-ttu-id="a0eab-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="a0eab-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0eab-124">Relações</span><span class="sxs-lookup"><span data-stu-id="a0eab-124">Relationships</span></span>
<span data-ttu-id="a0eab-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0eab-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0eab-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0eab-126">JSON Representation</span></span>
<span data-ttu-id="a0eab-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0eab-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



