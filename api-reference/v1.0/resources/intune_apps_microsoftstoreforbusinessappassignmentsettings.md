# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="33ef2-101">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="33ef2-101">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="33ef2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33ef2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33ef2-103">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="33ef2-103">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="33ef2-104">Herda de [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="33ef2-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33ef2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33ef2-105">Properties</span></span>
|<span data-ttu-id="33ef2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33ef2-106">Property</span></span>|<span data-ttu-id="33ef2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="33ef2-107">Type</span></span>|<span data-ttu-id="33ef2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="33ef2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33ef2-109">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="33ef2-109">useDeviceContext</span></span>|<span data-ttu-id="33ef2-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="33ef2-110">Boolean</span></span>|<span data-ttu-id="33ef2-111">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="33ef2-111">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33ef2-112">Relações</span><span class="sxs-lookup"><span data-stu-id="33ef2-112">Relationships</span></span>
<span data-ttu-id="33ef2-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33ef2-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33ef2-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33ef2-114">JSON Representation</span></span>
<span data-ttu-id="33ef2-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33ef2-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



