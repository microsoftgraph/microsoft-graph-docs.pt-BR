# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="932cd-101">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="932cd-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="932cd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="932cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="932cd-103">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="932cd-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="932cd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="932cd-104">Properties</span></span>
|<span data-ttu-id="932cd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="932cd-105">Property</span></span>|<span data-ttu-id="932cd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="932cd-106">Type</span></span>|<span data-ttu-id="932cd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="932cd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="932cd-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="932cd-108">v8_0</span></span>|<span data-ttu-id="932cd-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="932cd-109">Boolean</span></span>|<span data-ttu-id="932cd-110">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="932cd-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="932cd-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="932cd-111">v8_1</span></span>|<span data-ttu-id="932cd-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="932cd-112">Boolean</span></span>|<span data-ttu-id="932cd-113">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="932cd-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="932cd-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="932cd-114">v10_0</span></span>|<span data-ttu-id="932cd-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="932cd-115">Boolean</span></span>|<span data-ttu-id="932cd-116">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="932cd-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="932cd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="932cd-117">Relationships</span></span>
<span data-ttu-id="932cd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="932cd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="932cd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="932cd-119">JSON Representation</span></span>
<span data-ttu-id="932cd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="932cd-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



