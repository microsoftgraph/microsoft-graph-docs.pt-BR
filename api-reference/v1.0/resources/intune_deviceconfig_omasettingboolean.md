# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="e9277-101">Tipo de recurso omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="e9277-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="e9277-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e9277-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9277-103">Definição booliana para configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="e9277-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="e9277-104">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e9277-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9277-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9277-105">Properties</span></span>
|<span data-ttu-id="e9277-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9277-106">Property</span></span>|<span data-ttu-id="e9277-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9277-107">Type</span></span>|<span data-ttu-id="e9277-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9277-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9277-109">displayName</span><span class="sxs-lookup"><span data-stu-id="e9277-109">displayName</span></span>|<span data-ttu-id="e9277-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9277-110">String</span></span>|<span data-ttu-id="e9277-111">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e9277-111">Display Name.</span></span> <span data-ttu-id="e9277-112">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e9277-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="e9277-113">descrição</span><span class="sxs-lookup"><span data-stu-id="e9277-113">description</span></span>|<span data-ttu-id="e9277-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9277-114">String</span></span>|<span data-ttu-id="e9277-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="e9277-115">Description.</span></span> <span data-ttu-id="e9277-116">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e9277-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="e9277-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="e9277-117">omaUri</span></span>|<span data-ttu-id="e9277-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9277-118">String</span></span>|<span data-ttu-id="e9277-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="e9277-119">OMA.</span></span> <span data-ttu-id="e9277-120">Herda de [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e9277-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="e9277-121">valor</span><span class="sxs-lookup"><span data-stu-id="e9277-121">value</span></span>|<span data-ttu-id="e9277-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9277-122">Boolean</span></span>|<span data-ttu-id="e9277-123">Valor.</span><span class="sxs-lookup"><span data-stu-id="e9277-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9277-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e9277-124">Relationships</span></span>
<span data-ttu-id="e9277-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9277-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9277-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9277-126">JSON Representation</span></span>
<span data-ttu-id="e9277-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9277-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```








