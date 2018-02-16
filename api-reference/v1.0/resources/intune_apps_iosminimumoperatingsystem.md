# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="80ee3-101">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80ee3-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="80ee3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="80ee3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80ee3-103">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="80ee3-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="80ee3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80ee3-104">Properties</span></span>
|<span data-ttu-id="80ee3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80ee3-105">Property</span></span>|<span data-ttu-id="80ee3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ee3-106">Type</span></span>|<span data-ttu-id="80ee3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ee3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80ee3-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="80ee3-108">v8_0</span></span>|<span data-ttu-id="80ee3-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="80ee3-109">Boolean</span></span>|<span data-ttu-id="80ee3-110">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="80ee3-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="80ee3-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="80ee3-111">v9_0</span></span>|<span data-ttu-id="80ee3-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="80ee3-112">Boolean</span></span>|<span data-ttu-id="80ee3-113">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="80ee3-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="80ee3-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="80ee3-114">v10_0</span></span>|<span data-ttu-id="80ee3-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="80ee3-115">Boolean</span></span>|<span data-ttu-id="80ee3-116">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="80ee3-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="80ee3-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="80ee3-117">v11_0</span></span>|<span data-ttu-id="80ee3-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="80ee3-118">Boolean</span></span>|<span data-ttu-id="80ee3-119">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="80ee3-119">Version 11.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80ee3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="80ee3-120">Relationships</span></span>
<span data-ttu-id="80ee3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80ee3-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80ee3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80ee3-122">JSON Representation</span></span>
<span data-ttu-id="80ee3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80ee3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```



