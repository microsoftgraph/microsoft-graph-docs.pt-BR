# <a name="devicecategory-resource-type"></a><span data-ttu-id="23e8f-101">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="23e8f-101">deviceCategory resource type</span></span>

> <span data-ttu-id="23e8f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23e8f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23e8f-103">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="23e8f-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="23e8f-104">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="23e8f-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="23e8f-105">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23e8f-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="23e8f-106">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23e8f-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="23e8f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="23e8f-107">Methods</span></span>
|<span data-ttu-id="23e8f-108">Método</span><span class="sxs-lookup"><span data-stu-id="23e8f-108">Method</span></span>|<span data-ttu-id="23e8f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23e8f-109">Return Type</span></span>|<span data-ttu-id="23e8f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e8f-111">Objetos [List deviceCategories](../api/intune_shared_devicecategory_list.md).</span><span class="sxs-lookup"><span data-stu-id="23e8f-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) objects.</span></span>|
|<span data-ttu-id="23e8f-112">Objeto [Get deviceCategory](../api/intune_shared_devicecategory_get.md).</span><span class="sxs-lookup"><span data-stu-id="23e8f-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) object.</span></span>|
|<span data-ttu-id="23e8f-113">Objeto [Create deviceCategory](../api/intune_shared_devicecategory_create.md).</span><span class="sxs-lookup"><span data-stu-id="23e8f-113">Create a new [deviceCategory](../api/intune_shared_devicecategory_create.md) object.</span></span>|
|<span data-ttu-id="23e8f-114">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span><span class="sxs-lookup"><span data-stu-id="23e8f-114">Delete deviceCategory</span></span>|
|<span data-ttu-id="23e8f-115">Objeto [Update deviceCategory](../api/intune_shared_devicecategory_update.md).</span><span class="sxs-lookup"><span data-stu-id="23e8f-115">Update the properties of a [deviceCategory](../api/intune_shared_devicecategory_update.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23e8f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23e8f-116">Properties</span></span>
|<span data-ttu-id="23e8f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23e8f-117">Property</span></span>|<span data-ttu-id="23e8f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="23e8f-118">Type</span></span>|<span data-ttu-id="23e8f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e8f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e8f-120">id</span><span class="sxs-lookup"><span data-stu-id="23e8f-120">id</span></span>|<span data-ttu-id="23e8f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23e8f-121">String</span></span>|<span data-ttu-id="23e8f-122">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23e8f-122">Unique identifier for the device category.</span></span> <span data-ttu-id="23e8f-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23e8f-123">Read-only.</span></span>|
|<span data-ttu-id="23e8f-124">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="23e8f-124">**On-boarding**</span></span>|
|<span data-ttu-id="23e8f-125">displayName</span><span class="sxs-lookup"><span data-stu-id="23e8f-125">displayName</span></span>|<span data-ttu-id="23e8f-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23e8f-126">String</span></span>|<span data-ttu-id="23e8f-127">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23e8f-127">Display name for the device category.</span></span>|
|<span data-ttu-id="23e8f-128">descrição</span><span class="sxs-lookup"><span data-stu-id="23e8f-128">description</span></span>|<span data-ttu-id="23e8f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23e8f-129">String</span></span>|<span data-ttu-id="23e8f-130">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23e8f-130">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23e8f-131">Relações</span><span class="sxs-lookup"><span data-stu-id="23e8f-131">Relationships</span></span>
<span data-ttu-id="23e8f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23e8f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23e8f-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23e8f-133">JSON Representation</span></span>
<span data-ttu-id="23e8f-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23e8f-134">Here is a JSON representation of the resource.</span></span>
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



