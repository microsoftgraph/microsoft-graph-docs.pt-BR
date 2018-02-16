# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3b328-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b328-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3b328-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b328-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b328-103">O recurso deviceManagement representa as identidades de dispositivos da coleção do locatário pré-configuradas no Intune e os perfis de registro que podem ser atribuídos às identidades de dispositivos com suporte para configuração de pré-registro.</span><span class="sxs-lookup"><span data-stu-id="3b328-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="3b328-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b328-104">Methods</span></span>
|<span data-ttu-id="3b328-105">Método</span><span class="sxs-lookup"><span data-stu-id="3b328-105">Method</span></span>|<span data-ttu-id="3b328-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b328-106">Return Type</span></span>|<span data-ttu-id="3b328-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b328-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b328-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b328-108">Get deviceManagement</span></span>](../api/intune_corpenrollment_devicemanagement_get.md)|[<span data-ttu-id="3b328-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b328-109">deviceManagement</span></span>](../resources/intune_corpenrollment_devicemanagement.md)|<span data-ttu-id="3b328-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_corpenrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3b328-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_corpenrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3b328-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b328-111">Update deviceManagement</span></span>](../api/intune_corpenrollment_devicemanagement_update.md)|[<span data-ttu-id="3b328-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b328-112">deviceManagement</span></span>](../resources/intune_corpenrollment_devicemanagement.md)|<span data-ttu-id="3b328-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_corpenrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3b328-113">Update the properties of a [calendar](../resources/intune_corpenrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b328-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b328-114">Properties</span></span>
|<span data-ttu-id="3b328-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b328-115">Property</span></span>|<span data-ttu-id="3b328-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b328-116">Type</span></span>|<span data-ttu-id="3b328-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b328-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b328-118">id</span><span class="sxs-lookup"><span data-stu-id="3b328-118">id</span></span>|<span data-ttu-id="3b328-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b328-119">String</span></span>|<span data-ttu-id="3b328-120">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="3b328-120">The resource GUID for the security object is not valid.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b328-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3b328-121">Relationships</span></span>
<span data-ttu-id="3b328-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b328-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b328-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b328-123">JSON Representation</span></span>
<span data-ttu-id="3b328-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b328-124">Here is a JSON representation of the resource.</span></span>
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



