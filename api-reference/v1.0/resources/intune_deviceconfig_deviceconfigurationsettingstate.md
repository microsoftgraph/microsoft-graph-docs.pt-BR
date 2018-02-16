# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="b5ee2-101">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="b5ee2-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b5ee2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5ee2-103">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="b5ee2-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5ee2-104">Properties</span></span>
|<span data-ttu-id="b5ee2-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5ee2-105">Property</span></span>|<span data-ttu-id="b5ee2-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5ee2-106">Type</span></span>|<span data-ttu-id="b5ee2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ee2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ee2-108">configuração</span><span class="sxs-lookup"><span data-stu-id="b5ee2-108">Setting</span></span>|<span data-ttu-id="b5ee2-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-109">String</span></span>|<span data-ttu-id="b5ee2-110">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="b5ee2-110">The setting that is being reported</span></span>|
|<span data-ttu-id="b5ee2-111">settingName</span><span class="sxs-lookup"><span data-stu-id="b5ee2-111">settingName</span></span>|<span data-ttu-id="b5ee2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-112">String</span></span>|<span data-ttu-id="b5ee2-113">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="b5ee2-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b5ee2-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b5ee2-114">instanceDisplayName</span></span>|<span data-ttu-id="b5ee2-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-115">String</span></span>|<span data-ttu-id="b5ee2-116">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b5ee2-117">estado</span><span class="sxs-lookup"><span data-stu-id="b5ee2-117">state</span></span>|<span data-ttu-id="b5ee2-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-118">String</span></span>|<span data-ttu-id="b5ee2-119">O estado de conformidade da configuração Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="b5ee2-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="b5ee2-120">Error.code</span></span>|<span data-ttu-id="b5ee2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b5ee2-121">Int64</span></span>|<span data-ttu-id="b5ee2-122">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="b5ee2-122">Error code for the setting</span></span>|
|<span data-ttu-id="b5ee2-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b5ee2-123">error_description</span></span>|<span data-ttu-id="b5ee2-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-124">String</span></span>|<span data-ttu-id="b5ee2-125">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="b5ee2-125">Error Description</span></span>|
|<span data-ttu-id="b5ee2-126">userId</span><span class="sxs-lookup"><span data-stu-id="b5ee2-126">userId</span></span>|<span data-ttu-id="b5ee2-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-127">String</span></span>|<span data-ttu-id="b5ee2-128">UserId</span><span class="sxs-lookup"><span data-stu-id="b5ee2-128">userId</span></span>|
|<span data-ttu-id="b5ee2-129">userName</span><span class="sxs-lookup"><span data-stu-id="b5ee2-129">UserName</span></span>|<span data-ttu-id="b5ee2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-130">String</span></span>|<span data-ttu-id="b5ee2-131">UserName</span><span class="sxs-lookup"><span data-stu-id="b5ee2-131">UserName</span></span>|
|<span data-ttu-id="b5ee2-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="b5ee2-132">userEmail</span></span>|<span data-ttu-id="b5ee2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-133">String</span></span>|<span data-ttu-id="b5ee2-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b5ee2-134">UserEmail</span></span>|
|<span data-ttu-id="b5ee2-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5ee2-135">userPrincipalName</span></span>|<span data-ttu-id="b5ee2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-136">String</span></span>|<span data-ttu-id="b5ee2-137">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-137">userPrincipalName</span></span>|
|<span data-ttu-id="b5ee2-138">fontes</span><span class="sxs-lookup"><span data-stu-id="b5ee2-138">Data sources:</span></span>|<span data-ttu-id="b5ee2-139">Conjunto [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b5ee2-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="b5ee2-140">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="b5ee2-140">Contributing policies</span></span>|
|<span data-ttu-id="b5ee2-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="b5ee2-141">currentValue</span></span>|<span data-ttu-id="b5ee2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ee2-142">String</span></span>|<span data-ttu-id="b5ee2-143">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="b5ee2-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5ee2-144">Relações</span><span class="sxs-lookup"><span data-stu-id="b5ee2-144">Relationships</span></span>
<span data-ttu-id="b5ee2-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5ee2-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5ee2-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5ee2-146">JSON Representation</span></span>
<span data-ttu-id="b5ee2-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5ee2-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



