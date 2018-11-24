# <a name="organization-resource-type"></a><span data-ttu-id="48e51-101">tipo de recurso da organização</span><span class="sxs-lookup"><span data-stu-id="48e51-101">organization resource type</span></span>

> <span data-ttu-id="48e51-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48e51-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48e51-103">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="48e51-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="48e51-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="48e51-104">Methods</span></span>
|<span data-ttu-id="48e51-105">Método</span><span class="sxs-lookup"><span data-stu-id="48e51-105">Method</span></span>|<span data-ttu-id="48e51-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48e51-106">Return Type</span></span>|<span data-ttu-id="48e51-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e51-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48e51-108">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="48e51-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="48e51-109">Coleção [organization](../resources/intune_onboarding_organization.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="48e51-110">Listar propriedades e relações de objetos de [organização](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="48e51-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="48e51-111">Obter organização</span><span class="sxs-lookup"><span data-stu-id="48e51-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="48e51-112">organização</span><span class="sxs-lookup"><span data-stu-id="48e51-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="48e51-113">Ler propriedades e relações de objetos de [organização](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="48e51-113">Read properties and relationships of the [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="48e51-114">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="48e51-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="48e51-115">organização</span><span class="sxs-lookup"><span data-stu-id="48e51-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="48e51-116">Atualizar as propriedades de um objeto de [organização](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="48e51-116">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="48e51-117">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="48e51-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="48e51-118">Int32</span><span class="sxs-lookup"><span data-stu-id="48e51-118">Int32</span></span>|<span data-ttu-id="48e51-119">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="48e51-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="48e51-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48e51-120">Properties</span></span>
|<span data-ttu-id="48e51-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48e51-121">Property</span></span>|<span data-ttu-id="48e51-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e51-122">Type</span></span>|<span data-ttu-id="48e51-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e51-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e51-124">id</span><span class="sxs-lookup"><span data-stu-id="48e51-124">id</span></span>|<span data-ttu-id="48e51-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e51-125">String</span></span>|<span data-ttu-id="48e51-126">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="48e51-126">The GUID for the object.</span></span>|
|<span data-ttu-id="48e51-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="48e51-127">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="48e51-128">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="48e51-128">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="48e51-129">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="48e51-129">Mobile device management authority.</span></span> <span data-ttu-id="48e51-130">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="48e51-130">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48e51-131">Relações</span><span class="sxs-lookup"><span data-stu-id="48e51-131">Relationships</span></span>
<span data-ttu-id="48e51-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48e51-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48e51-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48e51-133">JSON Representation</span></span>
<span data-ttu-id="48e51-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48e51-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->

