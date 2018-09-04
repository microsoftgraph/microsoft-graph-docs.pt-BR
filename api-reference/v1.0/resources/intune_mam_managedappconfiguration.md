# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="44204-101">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="44204-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="44204-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="44204-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44204-103">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="44204-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="44204-104">Herda de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="44204-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="44204-105">Methods</span></span>
|<span data-ttu-id="44204-106">Método</span><span class="sxs-lookup"><span data-stu-id="44204-106">Method</span></span>|<span data-ttu-id="44204-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="44204-107">Return Type</span></span>|<span data-ttu-id="44204-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="44204-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44204-109">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="44204-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="44204-110">Coleção [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44204-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="44204-111">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44204-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="44204-112">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="44204-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="44204-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="44204-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="44204-114">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44204-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44204-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44204-115">Properties</span></span>
|<span data-ttu-id="44204-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44204-116">Property</span></span>|<span data-ttu-id="44204-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="44204-117">Type</span></span>|<span data-ttu-id="44204-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="44204-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44204-119">displayName</span><span class="sxs-lookup"><span data-stu-id="44204-119">displayName</span></span>|<span data-ttu-id="44204-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44204-120">String</span></span>|<span data-ttu-id="44204-121">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="44204-121">Policy display name.</span></span> <span data-ttu-id="44204-122">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-123">description</span><span class="sxs-lookup"><span data-stu-id="44204-123">description</span></span>|<span data-ttu-id="44204-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44204-124">String</span></span>|<span data-ttu-id="44204-125">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="44204-125">The policy's description.</span></span> <span data-ttu-id="44204-126">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44204-127">createdDateTime</span></span>|<span data-ttu-id="44204-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44204-128">DateTimeOffset</span></span>|<span data-ttu-id="44204-129">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="44204-129">The date and time the policy was created.</span></span> <span data-ttu-id="44204-130">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44204-131">lastModifiedDateTime</span></span>|<span data-ttu-id="44204-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44204-132">DateTimeOffset</span></span>|<span data-ttu-id="44204-133">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="44204-133">Last time the policy was modified.</span></span> <span data-ttu-id="44204-134">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-135">id</span><span class="sxs-lookup"><span data-stu-id="44204-135">id</span></span>|<span data-ttu-id="44204-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44204-136">String</span></span>|<span data-ttu-id="44204-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44204-137">Key of the entity.</span></span> <span data-ttu-id="44204-138">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-139">version</span><span class="sxs-lookup"><span data-stu-id="44204-139">version</span></span>|<span data-ttu-id="44204-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44204-140">String</span></span>|<span data-ttu-id="44204-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="44204-141">Version of the entity.</span></span> <span data-ttu-id="44204-142">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="44204-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="44204-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="44204-143">customSettings</span></span>|<span data-ttu-id="44204-144">Coleção [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="44204-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="44204-145">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="44204-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="44204-146">Relações</span><span class="sxs-lookup"><span data-stu-id="44204-146">Relationships</span></span>
<span data-ttu-id="44204-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44204-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44204-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44204-148">JSON Representation</span></span>
<span data-ttu-id="44204-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44204-149">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}-->
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



