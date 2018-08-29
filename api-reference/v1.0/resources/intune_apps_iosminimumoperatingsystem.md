# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="85e54-101">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="85e54-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="85e54-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85e54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85e54-103">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="85e54-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="85e54-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85e54-104">Properties</span></span>
|<span data-ttu-id="85e54-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85e54-105">Property</span></span>|<span data-ttu-id="85e54-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="85e54-106">Type</span></span>|<span data-ttu-id="85e54-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="85e54-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e54-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="85e54-108">v8_0</span></span>|<span data-ttu-id="85e54-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="85e54-109">Boolean</span></span>|<span data-ttu-id="85e54-110">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="85e54-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="85e54-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="85e54-111">v9_0</span></span>|<span data-ttu-id="85e54-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="85e54-112">Boolean</span></span>|<span data-ttu-id="85e54-113">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="85e54-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="85e54-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="85e54-114">v10_0</span></span>|<span data-ttu-id="85e54-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="85e54-115">Boolean</span></span>|<span data-ttu-id="85e54-116">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="85e54-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="85e54-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="85e54-117">v11_0</span></span>|<span data-ttu-id="85e54-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="85e54-118">Boolean</span></span>|<span data-ttu-id="85e54-119">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="85e54-119">Version 11.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e54-120">Relações</span><span class="sxs-lookup"><span data-stu-id="85e54-120">Relationships</span></span>
<span data-ttu-id="85e54-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85e54-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85e54-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85e54-122">JSON Representation</span></span>
<span data-ttu-id="85e54-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85e54-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```



