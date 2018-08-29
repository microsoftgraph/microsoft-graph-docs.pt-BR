# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="2013d-101">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2013d-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="2013d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2013d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2013d-103">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="2013d-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="2013d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2013d-104">Properties</span></span>
|<span data-ttu-id="2013d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2013d-105">Property</span></span>|<span data-ttu-id="2013d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2013d-106">Type</span></span>|<span data-ttu-id="2013d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2013d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2013d-108">inventory</span><span class="sxs-lookup"><span data-stu-id="2013d-108">inventory</span></span>|<span data-ttu-id="2013d-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-109">Boolean</span></span>|<span data-ttu-id="2013d-110">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="2013d-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="2013d-111">modernApps</span></span>|<span data-ttu-id="2013d-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-112">Boolean</span></span>|<span data-ttu-id="2013d-113">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="2013d-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="2013d-114">resourceAccess</span></span>|<span data-ttu-id="2013d-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-115">Boolean</span></span>|<span data-ttu-id="2013d-116">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="2013d-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2013d-117">deviceConfiguration</span></span>|<span data-ttu-id="2013d-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-118">Boolean</span></span>|<span data-ttu-id="2013d-119">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="2013d-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2013d-120">compliancePolicy</span></span>|<span data-ttu-id="2013d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-121">Boolean</span></span>|<span data-ttu-id="2013d-122">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="2013d-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="2013d-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="2013d-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="2013d-124">Boolean</span></span>|<span data-ttu-id="2013d-125">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2013d-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="2013d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="2013d-126">Relationships</span></span>
<span data-ttu-id="2013d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2013d-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2013d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2013d-128">JSON Representation</span></span>
<span data-ttu-id="2013d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2013d-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}-->
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



