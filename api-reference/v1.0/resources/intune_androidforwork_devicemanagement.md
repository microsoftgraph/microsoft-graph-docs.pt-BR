# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3e49c-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3e49c-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3e49c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e49c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e49c-103">Entidade singleton que atua como um contêiner da funcionalidade de configurações do Android for Work no gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3e49c-103">Singleton entity that acts as a container for Android for Work settings functionality under device management.</span></span>
## <a name="methods"></a><span data-ttu-id="3e49c-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="3e49c-104">Methods</span></span>
|<span data-ttu-id="3e49c-105">Método</span><span class="sxs-lookup"><span data-stu-id="3e49c-105">Method</span></span>|<span data-ttu-id="3e49c-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e49c-106">Return Type</span></span>|<span data-ttu-id="3e49c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e49c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e49c-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3e49c-108">Get deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_get.md)|[<span data-ttu-id="3e49c-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3e49c-109">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="3e49c-110">Propriedades de leitura e relações do objeto [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3e49c-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3e49c-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3e49c-111">Update deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_update.md)|[<span data-ttu-id="3e49c-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3e49c-112">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="3e49c-113">Atualiza as propriedades de um objeto [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3e49c-113">Update the properties of a [calendar](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e49c-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e49c-114">Properties</span></span>
|<span data-ttu-id="3e49c-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e49c-115">Property</span></span>|<span data-ttu-id="3e49c-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e49c-116">Type</span></span>|<span data-ttu-id="3e49c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e49c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e49c-118">id</span><span class="sxs-lookup"><span data-stu-id="3e49c-118">id</span></span>|<span data-ttu-id="3e49c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e49c-119">String</span></span>|<span data-ttu-id="3e49c-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e49c-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e49c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3e49c-121">Relationships</span></span>
|<span data-ttu-id="3e49c-122">Relação</span><span class="sxs-lookup"><span data-stu-id="3e49c-122">Relationship</span></span>|<span data-ttu-id="3e49c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e49c-123">Type</span></span>|<span data-ttu-id="3e49c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e49c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e49c-125">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="3e49c-125">androidForWorkSettings</span></span>|[<span data-ttu-id="3e49c-126">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="3e49c-126">androidForWorkSettings</span></span>](../resources/intune_androidforwork_androidforworksettings.md)|<span data-ttu-id="3e49c-127">A entidade singleton de configurações do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="3e49c-127">The singleton Android for Work settings entity.</span></span>|
|<span data-ttu-id="3e49c-128">androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="3e49c-128">androidForWorkAppConfigurationSchemas</span></span>|<span data-ttu-id="3e49c-129">Coleção [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)</span><span class="sxs-lookup"><span data-stu-id="3e49c-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="3e49c-130">Entidades do esquema de configuração do aplicativo Android for Work.</span><span class="sxs-lookup"><span data-stu-id="3e49c-130">Android for Work app configuration schema entities.</span></span>|
|<span data-ttu-id="3e49c-131">androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="3e49c-131">androidForWorkEnrollmentProfiles</span></span>|<span data-ttu-id="3e49c-132">Coleção [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3e49c-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="3e49c-133">Entidades do perfil de registro do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="3e49c-133">Android for Work enrollment profile entities.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e49c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e49c-134">JSON Representation</span></span>
<span data-ttu-id="3e49c-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e49c-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



