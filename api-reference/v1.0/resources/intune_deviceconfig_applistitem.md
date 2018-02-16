# <a name="applistitem-resource-type"></a><span data-ttu-id="69002-101">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="69002-101">appListItem resource type</span></span>

> <span data-ttu-id="69002-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69002-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69002-103">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69002-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="69002-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69002-104">Properties</span></span>
|<span data-ttu-id="69002-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69002-105">Property</span></span>|<span data-ttu-id="69002-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="69002-106">Type</span></span>|<span data-ttu-id="69002-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="69002-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69002-108">name</span><span class="sxs-lookup"><span data-stu-id="69002-108">name</span></span>|<span data-ttu-id="69002-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69002-109">String</span></span>|<span data-ttu-id="69002-110">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69002-110">The application name.</span></span>|
|<span data-ttu-id="69002-111">distribuidor</span><span class="sxs-lookup"><span data-stu-id="69002-111">Publisher</span></span>|<span data-ttu-id="69002-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69002-112">String</span></span>|<span data-ttu-id="69002-113">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69002-113">The publisher of the application</span></span>|
|<span data-ttu-id="69002-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="69002-114">appStoreUrl</span></span>|<span data-ttu-id="69002-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69002-115">String</span></span>|<span data-ttu-id="69002-116">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69002-116">The URL of the add-in's web application.</span></span>|
|<span data-ttu-id="69002-117">appId</span><span class="sxs-lookup"><span data-stu-id="69002-117">appId</span></span>|<span data-ttu-id="69002-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69002-118">String</span></span>|<span data-ttu-id="69002-119">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69002-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="69002-120">Relações</span><span class="sxs-lookup"><span data-stu-id="69002-120">Relationships</span></span>
<span data-ttu-id="69002-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69002-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69002-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69002-122">JSON Representation</span></span>
<span data-ttu-id="69002-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69002-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



