# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="37400-101">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="37400-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="37400-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37400-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37400-103">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="37400-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="37400-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="37400-104">Methods</span></span>
|<span data-ttu-id="37400-105">Método</span><span class="sxs-lookup"><span data-stu-id="37400-105">Method</span></span>|<span data-ttu-id="37400-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37400-106">Return Type</span></span>|<span data-ttu-id="37400-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="37400-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37400-108">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="37400-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="37400-109">Conjunto [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="37400-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="37400-110">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="37400-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="37400-111">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="37400-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="37400-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="37400-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="37400-113">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="37400-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="37400-114">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="37400-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="37400-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37400-115">None</span></span>|<span data-ttu-id="37400-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="37400-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="37400-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37400-117">Properties</span></span>
|<span data-ttu-id="37400-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37400-118">Property</span></span>|<span data-ttu-id="37400-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="37400-119">Type</span></span>|<span data-ttu-id="37400-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37400-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37400-121">displayName</span><span class="sxs-lookup"><span data-stu-id="37400-121">displayName</span></span>|<span data-ttu-id="37400-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37400-122">String</span></span>|<span data-ttu-id="37400-123">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="37400-123">Policy display name.</span></span>|
|<span data-ttu-id="37400-124">descrição</span><span class="sxs-lookup"><span data-stu-id="37400-124">description</span></span>|<span data-ttu-id="37400-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37400-125">String</span></span>|<span data-ttu-id="37400-126">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="37400-126">The policy's description.</span></span>|
|<span data-ttu-id="37400-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37400-127">createdDateTime</span></span>|<span data-ttu-id="37400-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37400-128">DateTimeOffset</span></span>|<span data-ttu-id="37400-129">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="37400-129">The date and time the group was created.</span></span>|
|<span data-ttu-id="37400-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37400-130">lastModifiedDateTime</span></span>|<span data-ttu-id="37400-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37400-131">DateTimeOffset</span></span>|<span data-ttu-id="37400-132">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="37400-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="37400-133">id</span><span class="sxs-lookup"><span data-stu-id="37400-133">id</span></span>|<span data-ttu-id="37400-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37400-134">String</span></span>|<span data-ttu-id="37400-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37400-135">Key of the setting.</span></span>|
|<span data-ttu-id="37400-136">versão</span><span class="sxs-lookup"><span data-stu-id="37400-136">version</span></span>|<span data-ttu-id="37400-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37400-137">String</span></span>|<span data-ttu-id="37400-138">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="37400-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37400-139">Relações</span><span class="sxs-lookup"><span data-stu-id="37400-139">Relationships</span></span>
<span data-ttu-id="37400-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37400-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37400-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37400-141">JSON Representation</span></span>
<span data-ttu-id="37400-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37400-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



