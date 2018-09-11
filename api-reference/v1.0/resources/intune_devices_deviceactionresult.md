# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="78faf-101">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="78faf-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="78faf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="78faf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78faf-103">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="78faf-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="78faf-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78faf-104">Properties</span></span>
|<span data-ttu-id="78faf-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78faf-105">Property</span></span>|<span data-ttu-id="78faf-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="78faf-106">Type</span></span>|<span data-ttu-id="78faf-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="78faf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78faf-108">actionName</span><span class="sxs-lookup"><span data-stu-id="78faf-108">actionName</span></span>|<span data-ttu-id="78faf-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78faf-109">String</span></span>|<span data-ttu-id="78faf-110">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="78faf-110">Action name</span></span>|
|<span data-ttu-id="78faf-111">actionState</span><span class="sxs-lookup"><span data-stu-id="78faf-111">actionState</span></span>|[<span data-ttu-id="78faf-112">actionState</span><span class="sxs-lookup"><span data-stu-id="78faf-112">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="78faf-p101">Estado da ação. Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="78faf-p101">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="78faf-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="78faf-115">startDateTime</span></span>|<span data-ttu-id="78faf-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78faf-116">DateTimeOffset</span></span>|<span data-ttu-id="78faf-117">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="78faf-117">Time the action was initiated</span></span>|
|<span data-ttu-id="78faf-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="78faf-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="78faf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78faf-119">DateTimeOffset</span></span>|<span data-ttu-id="78faf-120">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="78faf-120">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="78faf-121">Relações</span><span class="sxs-lookup"><span data-stu-id="78faf-121">Relationships</span></span>
<span data-ttu-id="78faf-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78faf-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78faf-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78faf-123">JSON Representation</span></span>
<span data-ttu-id="78faf-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78faf-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```








