# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="1ac1c-101">Tipo de recurso omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac1c-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="1ac1c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ac1c-103">Definição de datetime para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="1ac1c-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ac1c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ac1c-105">Properties</span></span>
|<span data-ttu-id="1ac1c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ac1c-106">Property</span></span>|<span data-ttu-id="1ac1c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ac1c-107">Type</span></span>|<span data-ttu-id="1ac1c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ac1c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ac1c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="1ac1c-109">displayName</span></span>|<span data-ttu-id="1ac1c-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ac1c-110">String</span></span>|<span data-ttu-id="1ac1c-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-111">Display Name</span></span> <span data-ttu-id="1ac1c-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="1ac1c-113">descrição</span><span class="sxs-lookup"><span data-stu-id="1ac1c-113">description</span></span>|<span data-ttu-id="1ac1c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ac1c-114">String</span></span>|<span data-ttu-id="1ac1c-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-115">Description.</span></span> <span data-ttu-id="1ac1c-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="1ac1c-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="1ac1c-117">omaUri</span></span>|<span data-ttu-id="1ac1c-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ac1c-118">String</span></span>|<span data-ttu-id="1ac1c-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-119">OMA.</span></span> <span data-ttu-id="1ac1c-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="1ac1c-121">value</span><span class="sxs-lookup"><span data-stu-id="1ac1c-121">value</span></span>|<span data-ttu-id="1ac1c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac1c-122">DateTimeOffset</span></span>|<span data-ttu-id="1ac1c-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ac1c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1ac1c-124">Relationships</span></span>
<span data-ttu-id="1ac1c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ac1c-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ac1c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ac1c-126">JSON Representation</span></span>
<span data-ttu-id="1ac1c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ac1c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



