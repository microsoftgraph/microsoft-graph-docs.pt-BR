# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="a6689-101">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a6689-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="a6689-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6689-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6689-103">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6689-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="a6689-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6689-104">Properties</span></span>
|<span data-ttu-id="a6689-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6689-105">Property</span></span>|<span data-ttu-id="a6689-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6689-106">Type</span></span>|<span data-ttu-id="a6689-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6689-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6689-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a6689-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="a6689-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a6689-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="a6689-110">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6689-110">Deployment of an app.</span></span>|
|<span data-ttu-id="a6689-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="a6689-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="a6689-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a6689-112">Int32</span></span>|<span data-ttu-id="a6689-113">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a6689-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6689-114">Relações</span><span class="sxs-lookup"><span data-stu-id="a6689-114">Relationships</span></span>
<span data-ttu-id="a6689-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6689-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6689-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6689-116">JSON Representation</span></span>
<span data-ttu-id="a6689-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6689-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```








