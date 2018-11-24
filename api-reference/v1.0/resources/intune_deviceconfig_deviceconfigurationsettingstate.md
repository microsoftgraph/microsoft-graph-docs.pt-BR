# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="a42fd-101">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="a42fd-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="a42fd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a42fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a42fd-103">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a42fd-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="a42fd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a42fd-104">Properties</span></span>
|<span data-ttu-id="a42fd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a42fd-105">Property</span></span>|<span data-ttu-id="a42fd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a42fd-106">Type</span></span>|<span data-ttu-id="a42fd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a42fd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a42fd-108">configuração</span><span class="sxs-lookup"><span data-stu-id="a42fd-108">setting</span></span>|<span data-ttu-id="a42fd-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-109">String</span></span>|<span data-ttu-id="a42fd-110">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="a42fd-110">The setting that is being reported</span></span>|
|<span data-ttu-id="a42fd-111">settingName</span><span class="sxs-lookup"><span data-stu-id="a42fd-111">settingName</span></span>|<span data-ttu-id="a42fd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-112">String</span></span>|<span data-ttu-id="a42fd-113">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="a42fd-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a42fd-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a42fd-114">instanceDisplayName</span></span>|<span data-ttu-id="a42fd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-115">String</span></span>|<span data-ttu-id="a42fd-116">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="a42fd-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a42fd-117">estado</span><span class="sxs-lookup"><span data-stu-id="a42fd-117">state</span></span>|[<span data-ttu-id="a42fd-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a42fd-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="a42fd-119">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="a42fd-119">The compliance state of the setting.</span></span> <span data-ttu-id="a42fd-120">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a42fd-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a42fd-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="a42fd-121">errorCode</span></span>|<span data-ttu-id="a42fd-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a42fd-122">Int64</span></span>|<span data-ttu-id="a42fd-123">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="a42fd-123">Error code for the setting</span></span>|
|<span data-ttu-id="a42fd-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a42fd-124">errorDescription</span></span>|<span data-ttu-id="a42fd-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-125">String</span></span>|<span data-ttu-id="a42fd-126">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="a42fd-126">Error description</span></span>|
|<span data-ttu-id="a42fd-127">userId</span><span class="sxs-lookup"><span data-stu-id="a42fd-127">userId</span></span>|<span data-ttu-id="a42fd-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-128">String</span></span>|<span data-ttu-id="a42fd-129">UserId</span><span class="sxs-lookup"><span data-stu-id="a42fd-129">UserId</span></span>|
|<span data-ttu-id="a42fd-130">userName</span><span class="sxs-lookup"><span data-stu-id="a42fd-130">userName</span></span>|<span data-ttu-id="a42fd-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-131">String</span></span>|<span data-ttu-id="a42fd-132">UserName</span><span class="sxs-lookup"><span data-stu-id="a42fd-132">UserName</span></span>|
|<span data-ttu-id="a42fd-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="a42fd-133">userEmail</span></span>|<span data-ttu-id="a42fd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-134">String</span></span>|<span data-ttu-id="a42fd-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a42fd-135">UserEmail</span></span>|
|<span data-ttu-id="a42fd-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a42fd-136">userPrincipalName</span></span>|<span data-ttu-id="a42fd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-137">String</span></span>|<span data-ttu-id="a42fd-138">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a42fd-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="a42fd-139">sources</span><span class="sxs-lookup"><span data-stu-id="a42fd-139">sources</span></span>|<span data-ttu-id="a42fd-140">Coleção [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a42fd-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="a42fd-141">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="a42fd-141">Contributing policies</span></span>|
|<span data-ttu-id="a42fd-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="a42fd-142">currentValue</span></span>|<span data-ttu-id="a42fd-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42fd-143">String</span></span>|<span data-ttu-id="a42fd-144">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="a42fd-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a42fd-145">Relações</span><span class="sxs-lookup"><span data-stu-id="a42fd-145">Relationships</span></span>
<span data-ttu-id="a42fd-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a42fd-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a42fd-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a42fd-147">JSON Representation</span></span>
<span data-ttu-id="a42fd-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a42fd-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



