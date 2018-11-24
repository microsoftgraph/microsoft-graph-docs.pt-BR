# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="eee5d-101">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="eee5d-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="eee5d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eee5d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eee5d-103">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="eee5d-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="eee5d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eee5d-104">Properties</span></span>
|<span data-ttu-id="eee5d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eee5d-105">Property</span></span>|<span data-ttu-id="eee5d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="eee5d-106">Type</span></span>|<span data-ttu-id="eee5d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee5d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee5d-108">iPad</span><span class="sxs-lookup"><span data-stu-id="eee5d-108">iPad</span></span>|<span data-ttu-id="eee5d-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="eee5d-109">Boolean</span></span>|<span data-ttu-id="eee5d-110">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="eee5d-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="eee5d-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="eee5d-111">iPhoneAndIPod</span></span>|<span data-ttu-id="eee5d-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="eee5d-112">Boolean</span></span>|<span data-ttu-id="eee5d-113">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="eee5d-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eee5d-114">Relações</span><span class="sxs-lookup"><span data-stu-id="eee5d-114">Relationships</span></span>
<span data-ttu-id="eee5d-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eee5d-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eee5d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eee5d-116">JSON Representation</span></span>
<span data-ttu-id="eee5d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eee5d-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



