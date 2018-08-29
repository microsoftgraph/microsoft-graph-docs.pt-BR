# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="9c783-101">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="9c783-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="9c783-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c783-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c783-103">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="9c783-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="9c783-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c783-104">Properties</span></span>
|<span data-ttu-id="9c783-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c783-105">Property</span></span>|<span data-ttu-id="9c783-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c783-106">Type</span></span>|<span data-ttu-id="9c783-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c783-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c783-108">displayName</span><span class="sxs-lookup"><span data-stu-id="9c783-108">displayName</span></span>|<span data-ttu-id="9c783-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c783-109">String</span></span>|<span data-ttu-id="9c783-110">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c783-110">App display name.</span></span>|
|<span data-ttu-id="9c783-111">descrição</span><span class="sxs-lookup"><span data-stu-id="9c783-111">description</span></span>|<span data-ttu-id="9c783-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c783-112">String</span></span>|<span data-ttu-id="9c783-113">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c783-113">The app's description.</span></span>|
|<span data-ttu-id="9c783-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="9c783-114">publisherName</span></span>|<span data-ttu-id="9c783-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c783-115">String</span></span>|<span data-ttu-id="9c783-116">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="9c783-116">The publisher name</span></span>|
|<span data-ttu-id="9c783-117">productName</span><span class="sxs-lookup"><span data-stu-id="9c783-117">productName</span></span>|<span data-ttu-id="9c783-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c783-118">String</span></span>|<span data-ttu-id="9c783-119">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="9c783-119">The product name.</span></span>|
|<span data-ttu-id="9c783-120">negado</span><span class="sxs-lookup"><span data-stu-id="9c783-120">denied</span></span>|<span data-ttu-id="9c783-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c783-121">Boolean</span></span>|<span data-ttu-id="9c783-122">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c783-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c783-123">Relações</span><span class="sxs-lookup"><span data-stu-id="9c783-123">Relationships</span></span>
<span data-ttu-id="9c783-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c783-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c783-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c783-125">JSON Representation</span></span>
<span data-ttu-id="9c783-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c783-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



