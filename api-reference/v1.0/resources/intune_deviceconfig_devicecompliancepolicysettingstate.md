# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="f977c-101">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="f977c-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="f977c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f977c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f977c-103">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f977c-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f977c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f977c-104">Properties</span></span>
|<span data-ttu-id="f977c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f977c-105">Property</span></span>|<span data-ttu-id="f977c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f977c-106">Type</span></span>|<span data-ttu-id="f977c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f977c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f977c-108">setting</span><span class="sxs-lookup"><span data-stu-id="f977c-108">Setting</span></span>|<span data-ttu-id="f977c-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-109">String</span></span>|<span data-ttu-id="f977c-110">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="f977c-110">The setting that is being reported</span></span>|
|<span data-ttu-id="f977c-111">settingName</span><span class="sxs-lookup"><span data-stu-id="f977c-111">settingName</span></span>|<span data-ttu-id="f977c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-112">String</span></span>|<span data-ttu-id="f977c-113">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="f977c-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f977c-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f977c-114">instanceDisplayName</span></span>|<span data-ttu-id="f977c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-115">String</span></span>|<span data-ttu-id="f977c-116">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="f977c-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f977c-117">state</span><span class="sxs-lookup"><span data-stu-id="f977c-117">state</span></span>|<span data-ttu-id="f977c-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-118">String</span></span>|<span data-ttu-id="f977c-119">O estado de conformidade da configuração. Os possíveis valores são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="f977c-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="f977c-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="f977c-120">Error.code</span></span>|<span data-ttu-id="f977c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f977c-121">Int64</span></span>|<span data-ttu-id="f977c-122">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="f977c-122">Error code for the setting</span></span>|
|<span data-ttu-id="f977c-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f977c-123">error_description</span></span>|<span data-ttu-id="f977c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-124">String</span></span>|<span data-ttu-id="f977c-125">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="f977c-125">Error Description</span></span>|
|<span data-ttu-id="f977c-126">userId</span><span class="sxs-lookup"><span data-stu-id="f977c-126">userId</span></span>|<span data-ttu-id="f977c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-127">String</span></span>|<span data-ttu-id="f977c-128">UserId</span><span class="sxs-lookup"><span data-stu-id="f977c-128">userId</span></span>|
|<span data-ttu-id="f977c-129">userName</span><span class="sxs-lookup"><span data-stu-id="f977c-129">UserName</span></span>|<span data-ttu-id="f977c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-130">String</span></span>|<span data-ttu-id="f977c-131">UserName</span><span class="sxs-lookup"><span data-stu-id="f977c-131">UserName</span></span>|
|<span data-ttu-id="f977c-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="f977c-132">userEmail</span></span>|<span data-ttu-id="f977c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-133">String</span></span>|<span data-ttu-id="f977c-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f977c-134">UserEmail</span></span>|
|<span data-ttu-id="f977c-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f977c-135">userPrincipalName</span></span>|<span data-ttu-id="f977c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-136">String</span></span>|<span data-ttu-id="f977c-137">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f977c-137">userPrincipalName</span></span>|
|<span data-ttu-id="f977c-138">sources</span><span class="sxs-lookup"><span data-stu-id="f977c-138">Data sources:</span></span>|<span data-ttu-id="f977c-139">Coleção [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="f977c-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="f977c-140">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="f977c-140">Contributing policies</span></span>|
|<span data-ttu-id="f977c-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="f977c-141">currentValue</span></span>|<span data-ttu-id="f977c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f977c-142">String</span></span>|<span data-ttu-id="f977c-143">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f977c-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f977c-144">Relações</span><span class="sxs-lookup"><span data-stu-id="f977c-144">Relationships</span></span>
<span data-ttu-id="f977c-145">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f977c-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f977c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f977c-146">JSON Representation</span></span>
<span data-ttu-id="f977c-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f977c-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



