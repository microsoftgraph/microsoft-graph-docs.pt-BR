# <a name="devicemanagement-resource-type"></a><span data-ttu-id="389d4-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="389d4-101">deviceManagement resource type</span></span>

> <span data-ttu-id="389d4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="389d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="389d4-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="389d4-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="389d4-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="389d4-104">Methods</span></span>
|<span data-ttu-id="389d4-105">Método</span><span class="sxs-lookup"><span data-stu-id="389d4-105">Method</span></span>|<span data-ttu-id="389d4-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="389d4-106">Return Type</span></span>|<span data-ttu-id="389d4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="389d4-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="389d4-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="389d4-108">Get deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_get.md)|[<span data-ttu-id="389d4-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="389d4-109">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="389d4-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_companyterms_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="389d4-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="389d4-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="389d4-111">Update deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_update.md)|[<span data-ttu-id="389d4-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="389d4-112">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="389d4-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_companyterms_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="389d4-113">Update the properties of a [calendar](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="389d4-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="389d4-114">Properties</span></span>
|<span data-ttu-id="389d4-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="389d4-115">Property</span></span>|<span data-ttu-id="389d4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="389d4-116">Type</span></span>|<span data-ttu-id="389d4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="389d4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="389d4-118">id</span><span class="sxs-lookup"><span data-stu-id="389d4-118">id</span></span>|<span data-ttu-id="389d4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="389d4-119">String</span></span>|<span data-ttu-id="389d4-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="389d4-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="389d4-121">Relações</span><span class="sxs-lookup"><span data-stu-id="389d4-121">Relationships</span></span>
|<span data-ttu-id="389d4-122">Relação</span><span class="sxs-lookup"><span data-stu-id="389d4-122">Relationship</span></span>|<span data-ttu-id="389d4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="389d4-123">Type</span></span>|<span data-ttu-id="389d4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="389d4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="389d4-125">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="389d4-125">termsAndConditions</span></span>|<span data-ttu-id="389d4-126">Conjunto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)</span><span class="sxs-lookup"><span data-stu-id="389d4-126">[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) collection</span></span>|<span data-ttu-id="389d4-127">Os termos e condições associados ao gerenciamento do dispositivo da empresa.</span><span class="sxs-lookup"><span data-stu-id="389d4-127">The terms and conditions associated with device management of the company.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="389d4-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="389d4-128">JSON Representation</span></span>
<span data-ttu-id="389d4-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="389d4-129">Here is a JSON representation of the resource.</span></span>
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



