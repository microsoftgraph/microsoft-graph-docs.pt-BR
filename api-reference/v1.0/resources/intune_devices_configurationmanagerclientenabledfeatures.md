# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="96bb1-101">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="96bb1-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="96bb1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96bb1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96bb1-103">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="96bb1-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="96bb1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96bb1-104">Properties</span></span>
|<span data-ttu-id="96bb1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96bb1-105">Property</span></span>|<span data-ttu-id="96bb1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bb1-106">Type</span></span>|<span data-ttu-id="96bb1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bb1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96bb1-108">inventory</span><span class="sxs-lookup"><span data-stu-id="96bb1-108">inventory</span></span>|<span data-ttu-id="96bb1-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-109">Boolean</span></span>|<span data-ttu-id="96bb1-110">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="96bb1-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="96bb1-111">modernApps</span></span>|<span data-ttu-id="96bb1-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-112">Boolean</span></span>|<span data-ttu-id="96bb1-113">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="96bb1-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="96bb1-114">resourceAccess</span></span>|<span data-ttu-id="96bb1-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-115">Boolean</span></span>|<span data-ttu-id="96bb1-116">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="96bb1-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="96bb1-117">deviceConfiguration</span></span>|<span data-ttu-id="96bb1-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-118">Boolean</span></span>|<span data-ttu-id="96bb1-119">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="96bb1-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="96bb1-120">compliancePolicy</span></span>|<span data-ttu-id="96bb1-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-121">Boolean</span></span>|<span data-ttu-id="96bb1-122">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="96bb1-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="96bb1-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="96bb1-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="96bb1-124">Boolean</span></span>|<span data-ttu-id="96bb1-125">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="96bb1-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="96bb1-126">Relações</span><span class="sxs-lookup"><span data-stu-id="96bb1-126">Relationships</span></span>
<span data-ttu-id="96bb1-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="96bb1-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96bb1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96bb1-128">JSON Representation</span></span>
<span data-ttu-id="96bb1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96bb1-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



