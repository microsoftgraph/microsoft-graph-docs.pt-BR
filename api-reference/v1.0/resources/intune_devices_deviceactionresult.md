# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="66de0-101">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="66de0-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="66de0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66de0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66de0-103">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="66de0-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="66de0-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66de0-104">Properties</span></span>
|<span data-ttu-id="66de0-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66de0-105">Property</span></span>|<span data-ttu-id="66de0-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="66de0-106">Type</span></span>|<span data-ttu-id="66de0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="66de0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66de0-108">actionName</span><span class="sxs-lookup"><span data-stu-id="66de0-108">actionName</span></span>|<span data-ttu-id="66de0-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66de0-109">String</span></span>|<span data-ttu-id="66de0-110">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="66de0-110">Action name</span></span>|
|<span data-ttu-id="66de0-111">actionState</span><span class="sxs-lookup"><span data-stu-id="66de0-111">actionState</span></span>|<span data-ttu-id="66de0-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66de0-112">String</span></span>|<span data-ttu-id="66de0-113">Estado da ação Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="66de0-113">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="66de0-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="66de0-114">startDateTime</span></span>|<span data-ttu-id="66de0-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66de0-115">DateTimeOffset</span></span>|<span data-ttu-id="66de0-116">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="66de0-116">Time the action was initiated</span></span>|
|<span data-ttu-id="66de0-117">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="66de0-117">lastUpdatedDateTime</span></span>|<span data-ttu-id="66de0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66de0-118">DateTimeOffset</span></span>|<span data-ttu-id="66de0-119">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="66de0-119">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="66de0-120">Relações</span><span class="sxs-lookup"><span data-stu-id="66de0-120">Relationships</span></span>
<span data-ttu-id="66de0-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66de0-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66de0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66de0-122">JSON Representation</span></span>
<span data-ttu-id="66de0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66de0-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



