# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="d57b6-101">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d57b6-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="d57b6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d57b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d57b6-103">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="d57b6-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="d57b6-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d57b6-104">Properties</span></span>
|<span data-ttu-id="d57b6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d57b6-105">Property</span></span>|<span data-ttu-id="d57b6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d57b6-106">Type</span></span>|<span data-ttu-id="d57b6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d57b6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57b6-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="d57b6-108">v8_0</span></span>|<span data-ttu-id="d57b6-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="d57b6-109">Boolean</span></span>|<span data-ttu-id="d57b6-110">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="d57b6-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="d57b6-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="d57b6-111">v8_1</span></span>|<span data-ttu-id="d57b6-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="d57b6-112">Boolean</span></span>|<span data-ttu-id="d57b6-113">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="d57b6-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="d57b6-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="d57b6-114">v10_0</span></span>|<span data-ttu-id="d57b6-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="d57b6-115">Boolean</span></span>|<span data-ttu-id="d57b6-116">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="d57b6-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d57b6-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d57b6-117">Relationships</span></span>
<span data-ttu-id="d57b6-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d57b6-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d57b6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d57b6-119">JSON Representation</span></span>
<span data-ttu-id="d57b6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d57b6-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



