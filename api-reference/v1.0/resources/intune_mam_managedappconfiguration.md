# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="8abf3-101">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8abf3-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="8abf3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8abf3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8abf3-103">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="8abf3-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="8abf3-104">Herda de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8abf3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8abf3-105">Methods</span></span>
|<span data-ttu-id="8abf3-106">Método</span><span class="sxs-lookup"><span data-stu-id="8abf3-106">Method</span></span>|<span data-ttu-id="8abf3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8abf3-107">Return Type</span></span>|<span data-ttu-id="8abf3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8abf3-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8abf3-109">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8abf3-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="8abf3-110">Coleção [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="8abf3-111">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8abf3-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8abf3-112">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8abf3-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="8abf3-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8abf3-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="8abf3-114">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8abf3-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8abf3-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8abf3-115">Properties</span></span>
|<span data-ttu-id="8abf3-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8abf3-116">Property</span></span>|<span data-ttu-id="8abf3-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8abf3-117">Type</span></span>|<span data-ttu-id="8abf3-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8abf3-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8abf3-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8abf3-119">displayName</span></span>|<span data-ttu-id="8abf3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8abf3-120">String</span></span>|<span data-ttu-id="8abf3-121">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="8abf3-121">Policy display name.</span></span> <span data-ttu-id="8abf3-122">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-123">description</span><span class="sxs-lookup"><span data-stu-id="8abf3-123">description</span></span>|<span data-ttu-id="8abf3-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8abf3-124">String</span></span>|<span data-ttu-id="8abf3-125">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="8abf3-125">The policy's description.</span></span> <span data-ttu-id="8abf3-126">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8abf3-127">createdDateTime</span></span>|<span data-ttu-id="8abf3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8abf3-128">DateTimeOffset</span></span>|<span data-ttu-id="8abf3-129">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="8abf3-129">The date and time the policy was created.</span></span> <span data-ttu-id="8abf3-130">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8abf3-131">lastModifiedDateTime</span></span>|<span data-ttu-id="8abf3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8abf3-132">DateTimeOffset</span></span>|<span data-ttu-id="8abf3-133">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="8abf3-133">Last time the policy was modified.</span></span> <span data-ttu-id="8abf3-134">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-135">id</span><span class="sxs-lookup"><span data-stu-id="8abf3-135">id</span></span>|<span data-ttu-id="8abf3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8abf3-136">String</span></span>|<span data-ttu-id="8abf3-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8abf3-137">Key of the entity.</span></span> <span data-ttu-id="8abf3-138">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-139">version</span><span class="sxs-lookup"><span data-stu-id="8abf3-139">version</span></span>|<span data-ttu-id="8abf3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8abf3-140">String</span></span>|<span data-ttu-id="8abf3-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8abf3-141">Version of the entity.</span></span> <span data-ttu-id="8abf3-142">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8abf3-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="8abf3-143">customSettings</span></span>|<span data-ttu-id="8abf3-144">Coleção [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8abf3-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="8abf3-145">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="8abf3-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="8abf3-146">Relações</span><span class="sxs-lookup"><span data-stu-id="8abf3-146">Relationships</span></span>
<span data-ttu-id="8abf3-147">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8abf3-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8abf3-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8abf3-148">JSON Representation</span></span>
<span data-ttu-id="8abf3-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8abf3-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



