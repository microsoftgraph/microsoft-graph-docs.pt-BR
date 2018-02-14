# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="b67fc-101">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="b67fc-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="b67fc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b67fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b67fc-103">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b67fc-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="b67fc-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b67fc-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b67fc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b67fc-105">Properties</span></span>
|<span data-ttu-id="b67fc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b67fc-106">Property</span></span>|<span data-ttu-id="b67fc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b67fc-107">Type</span></span>|<span data-ttu-id="b67fc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b67fc-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67fc-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b67fc-109">displayName</span></span>|<span data-ttu-id="b67fc-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67fc-110">String</span></span>|<span data-ttu-id="b67fc-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b67fc-111">Display Name</span></span> <span data-ttu-id="b67fc-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b67fc-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b67fc-113">descrição</span><span class="sxs-lookup"><span data-stu-id="b67fc-113">description</span></span>|<span data-ttu-id="b67fc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67fc-114">String</span></span>|<span data-ttu-id="b67fc-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b67fc-115">Description.</span></span> <span data-ttu-id="b67fc-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b67fc-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b67fc-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="b67fc-117">omaUri</span></span>|<span data-ttu-id="b67fc-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67fc-118">String</span></span>|<span data-ttu-id="b67fc-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="b67fc-119">OMA.</span></span> <span data-ttu-id="b67fc-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b67fc-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="b67fc-121">value</span><span class="sxs-lookup"><span data-stu-id="b67fc-121">value</span></span>|<span data-ttu-id="b67fc-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="b67fc-122">Boolean</span></span>|<span data-ttu-id="b67fc-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="b67fc-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b67fc-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b67fc-124">Relationships</span></span>
<span data-ttu-id="b67fc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b67fc-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b67fc-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b67fc-126">JSON Representation</span></span>
<span data-ttu-id="b67fc-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b67fc-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



