# <a name="devicecategory-resource-type"></a><span data-ttu-id="9ab02-101">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9ab02-101">deviceCategory resource type</span></span>

> <span data-ttu-id="9ab02-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ab02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ab02-103">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ab02-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="9ab02-104">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="9ab02-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="9ab02-105">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ab02-105"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="9ab02-106">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ab02-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="9ab02-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ab02-107">Methods</span></span>
|<span data-ttu-id="9ab02-108">Método</span><span class="sxs-lookup"><span data-stu-id="9ab02-108">Method</span></span>|<span data-ttu-id="9ab02-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ab02-109">Return Type</span></span>|<span data-ttu-id="9ab02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab02-111">Coleção da [lista deviceCategories](../api/intune_shared_devicecategory_list.md)</span><span class="sxs-lookup"><span data-stu-id="9ab02-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="9ab02-112">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9ab02-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="9ab02-113">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9ab02-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="9ab02-114">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9ab02-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="9ab02-115">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9ab02-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="9ab02-116">Cria um novo objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9ab02-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="9ab02-117">[Excluir deviceCategory](../api/intune_shared_devicecategory_delete.md).</span><span class="sxs-lookup"><span data-stu-id="9ab02-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span></span>|
|[<span data-ttu-id="9ab02-118">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9ab02-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="9ab02-119">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9ab02-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ab02-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ab02-120">Properties</span></span>
|<span data-ttu-id="9ab02-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ab02-121">Property</span></span>|<span data-ttu-id="9ab02-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ab02-122">Type</span></span>|<span data-ttu-id="9ab02-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab02-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab02-124">id</span><span class="sxs-lookup"><span data-stu-id="9ab02-124">id</span></span>|<span data-ttu-id="9ab02-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab02-125">String</span></span>|<span data-ttu-id="9ab02-126">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ab02-126">Unique identifier for the device category.</span></span> <span data-ttu-id="9ab02-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab02-127">Read-only.</span></span>|
|<span data-ttu-id="9ab02-128">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="9ab02-128">**Onboarding**</span></span>|
|<span data-ttu-id="9ab02-129">displayName</span><span class="sxs-lookup"><span data-stu-id="9ab02-129">displayName</span></span>|<span data-ttu-id="9ab02-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab02-130">String</span></span>|<span data-ttu-id="9ab02-131">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ab02-131">Display name for the device category.</span></span>|
|<span data-ttu-id="9ab02-132">description</span><span class="sxs-lookup"><span data-stu-id="9ab02-132">description</span></span>|<span data-ttu-id="9ab02-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab02-133">String</span></span>|<span data-ttu-id="9ab02-134">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ab02-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ab02-135">Relações</span><span class="sxs-lookup"><span data-stu-id="9ab02-135">Relationships</span></span>
<span data-ttu-id="9ab02-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ab02-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ab02-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ab02-137">JSON Representation</span></span>
<span data-ttu-id="9ab02-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ab02-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



