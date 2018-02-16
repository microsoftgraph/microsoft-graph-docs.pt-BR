# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="bc411-101">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bc411-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="bc411-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc411-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc411-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc411-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="bc411-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc411-104">Methods</span></span>
|<span data-ttu-id="bc411-105">Método</span><span class="sxs-lookup"><span data-stu-id="bc411-105">Method</span></span>|<span data-ttu-id="bc411-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc411-106">Return Type</span></span>|<span data-ttu-id="bc411-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc411-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc411-108">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bc411-108">Get deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_get.md)|[<span data-ttu-id="bc411-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bc411-109">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="bc411-110">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="bc411-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="bc411-111">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bc411-111">Update deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_update.md)|[<span data-ttu-id="bc411-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="bc411-112">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="bc411-113">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="bc411-113">Update the properties of a [calendar](../resources/intune_books_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc411-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc411-114">Properties</span></span>
|<span data-ttu-id="bc411-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc411-115">Property</span></span>|<span data-ttu-id="bc411-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc411-116">Type</span></span>|<span data-ttu-id="bc411-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc411-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc411-118">id</span><span class="sxs-lookup"><span data-stu-id="bc411-118">id</span></span>|<span data-ttu-id="bc411-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc411-119">String</span></span>|<span data-ttu-id="bc411-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc411-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc411-121">Relações</span><span class="sxs-lookup"><span data-stu-id="bc411-121">Relationships</span></span>
|<span data-ttu-id="bc411-122">Relação</span><span class="sxs-lookup"><span data-stu-id="bc411-122">Relationship</span></span>|<span data-ttu-id="bc411-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc411-123">Type</span></span>|<span data-ttu-id="bc411-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc411-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc411-125">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="bc411-125">managedEBooks</span></span>|<span data-ttu-id="bc411-126">Conjunto [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="bc411-126">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="bc411-127">Livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bc411-127">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc411-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc411-128">JSON Representation</span></span>
<span data-ttu-id="bc411-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc411-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



