# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="b4d72-101">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d72-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="b4d72-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4d72-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4d72-103">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="b4d72-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="b4d72-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4d72-104">Methods</span></span>
|<span data-ttu-id="b4d72-105">Método</span><span class="sxs-lookup"><span data-stu-id="b4d72-105">Method</span></span>|<span data-ttu-id="b4d72-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4d72-106">Return Type</span></span>|<span data-ttu-id="b4d72-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d72-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4d72-108">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="b4d72-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="b4d72-109">Conjunto [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b4d72-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="b4d72-110">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b4d72-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="b4d72-111">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d72-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="b4d72-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d72-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="b4d72-113">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b4d72-113">Read properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="b4d72-114">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="b4d72-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="b4d72-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4d72-115">None</span></span>|<span data-ttu-id="b4d72-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4d72-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b4d72-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4d72-117">Properties</span></span>
|<span data-ttu-id="b4d72-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4d72-118">Property</span></span>|<span data-ttu-id="b4d72-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4d72-119">Type</span></span>|<span data-ttu-id="b4d72-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d72-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d72-121">displayName</span><span class="sxs-lookup"><span data-stu-id="b4d72-121">displayName</span></span>|<span data-ttu-id="b4d72-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4d72-122">String</span></span>|<span data-ttu-id="b4d72-123">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="b4d72-123">Policy display name.</span></span>|
|<span data-ttu-id="b4d72-124">descrição</span><span class="sxs-lookup"><span data-stu-id="b4d72-124">description</span></span>|<span data-ttu-id="b4d72-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4d72-125">String</span></span>|<span data-ttu-id="b4d72-126">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="b4d72-126">The policy's description.</span></span>|
|<span data-ttu-id="b4d72-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4d72-127">createdDateTime</span></span>|<span data-ttu-id="b4d72-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4d72-128">DateTimeOffset</span></span>|<span data-ttu-id="b4d72-129">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="b4d72-129">The date and time the policy was created.</span></span>|
|<span data-ttu-id="b4d72-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4d72-130">lastModifiedDateTime</span></span>|<span data-ttu-id="b4d72-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4d72-131">DateTimeOffset</span></span>|<span data-ttu-id="b4d72-132">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="b4d72-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="b4d72-133">id</span><span class="sxs-lookup"><span data-stu-id="b4d72-133">id</span></span>|<span data-ttu-id="b4d72-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4d72-134">String</span></span>|<span data-ttu-id="b4d72-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4d72-135">Key of the entity.</span></span>|
|<span data-ttu-id="b4d72-136">version</span><span class="sxs-lookup"><span data-stu-id="b4d72-136">version</span></span>|<span data-ttu-id="b4d72-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4d72-137">String</span></span>|<span data-ttu-id="b4d72-138">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4d72-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4d72-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b4d72-139">Relationships</span></span>
<span data-ttu-id="b4d72-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4d72-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b4d72-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4d72-141">JSON Representation</span></span>
<span data-ttu-id="b4d72-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4d72-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}-->
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



