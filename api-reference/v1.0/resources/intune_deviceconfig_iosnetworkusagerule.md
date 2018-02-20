# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="0bc1f-101">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="0bc1f-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="0bc1f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bc1f-103">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="0bc1f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bc1f-104">Properties</span></span>
|<span data-ttu-id="0bc1f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc1f-105">Property</span></span>|<span data-ttu-id="0bc1f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc1f-106">Type</span></span>|<span data-ttu-id="0bc1f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc1f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc1f-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="0bc1f-108">managedApps</span></span>|<span data-ttu-id="0bc1f-109">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0bc1f-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="0bc1f-110">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="0bc1f-111">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0bc1f-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="0bc1f-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="0bc1f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bc1f-113">Boolean</span></span>|<span data-ttu-id="0bc1f-114">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="0bc1f-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="0bc1f-115">cellularDataBlocked</span></span>|<span data-ttu-id="0bc1f-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bc1f-116">Boolean</span></span>|<span data-ttu-id="0bc1f-117">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bc1f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0bc1f-118">Relationships</span></span>
<span data-ttu-id="0bc1f-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0bc1f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0bc1f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bc1f-120">JSON Representation</span></span>
<span data-ttu-id="0bc1f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



