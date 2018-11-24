# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="73fc1-101">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="73fc1-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="73fc1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="73fc1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73fc1-103">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73fc1-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="73fc1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73fc1-104">Properties</span></span>
|<span data-ttu-id="73fc1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73fc1-105">Property</span></span>|<span data-ttu-id="73fc1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="73fc1-106">Type</span></span>|<span data-ttu-id="73fc1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="73fc1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73fc1-108">setting</span><span class="sxs-lookup"><span data-stu-id="73fc1-108">setting</span></span>|<span data-ttu-id="73fc1-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-109">String</span></span>|<span data-ttu-id="73fc1-110">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="73fc1-110">The setting that is being reported</span></span>|
|<span data-ttu-id="73fc1-111">settingName</span><span class="sxs-lookup"><span data-stu-id="73fc1-111">settingName</span></span>|<span data-ttu-id="73fc1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-112">String</span></span>|<span data-ttu-id="73fc1-113">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="73fc1-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="73fc1-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="73fc1-114">instanceDisplayName</span></span>|<span data-ttu-id="73fc1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-115">String</span></span>|<span data-ttu-id="73fc1-116">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="73fc1-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="73fc1-117">state</span><span class="sxs-lookup"><span data-stu-id="73fc1-117">state</span></span>|[<span data-ttu-id="73fc1-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="73fc1-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="73fc1-119">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="73fc1-119">The compliance state of the setting.</span></span> <span data-ttu-id="73fc1-120">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="73fc1-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="73fc1-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="73fc1-121">errorCode</span></span>|<span data-ttu-id="73fc1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="73fc1-122">Int64</span></span>|<span data-ttu-id="73fc1-123">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="73fc1-123">Error code for the setting</span></span>|
|<span data-ttu-id="73fc1-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="73fc1-124">errorDescription</span></span>|<span data-ttu-id="73fc1-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-125">String</span></span>|<span data-ttu-id="73fc1-126">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="73fc1-126">Error description</span></span>|
|<span data-ttu-id="73fc1-127">userId</span><span class="sxs-lookup"><span data-stu-id="73fc1-127">userId</span></span>|<span data-ttu-id="73fc1-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-128">String</span></span>|<span data-ttu-id="73fc1-129">UserId</span><span class="sxs-lookup"><span data-stu-id="73fc1-129">UserId</span></span>|
|<span data-ttu-id="73fc1-130">userName</span><span class="sxs-lookup"><span data-stu-id="73fc1-130">userName</span></span>|<span data-ttu-id="73fc1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-131">String</span></span>|<span data-ttu-id="73fc1-132">UserName</span><span class="sxs-lookup"><span data-stu-id="73fc1-132">UserName</span></span>|
|<span data-ttu-id="73fc1-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="73fc1-133">userEmail</span></span>|<span data-ttu-id="73fc1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-134">String</span></span>|<span data-ttu-id="73fc1-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="73fc1-135">UserEmail</span></span>|
|<span data-ttu-id="73fc1-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="73fc1-136">userPrincipalName</span></span>|<span data-ttu-id="73fc1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-137">String</span></span>|<span data-ttu-id="73fc1-138">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="73fc1-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="73fc1-139">sources</span><span class="sxs-lookup"><span data-stu-id="73fc1-139">sources</span></span>|<span data-ttu-id="73fc1-140">Coleção [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="73fc1-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="73fc1-141">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="73fc1-141">Contributing policies</span></span>|
|<span data-ttu-id="73fc1-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="73fc1-142">currentValue</span></span>|<span data-ttu-id="73fc1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73fc1-143">String</span></span>|<span data-ttu-id="73fc1-144">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="73fc1-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="73fc1-145">Relações</span><span class="sxs-lookup"><span data-stu-id="73fc1-145">Relationships</span></span>
<span data-ttu-id="73fc1-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73fc1-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73fc1-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73fc1-147">JSON Representation</span></span>
<span data-ttu-id="73fc1-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73fc1-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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



