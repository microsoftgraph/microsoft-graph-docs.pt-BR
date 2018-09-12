# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="708c6-101">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="708c6-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="708c6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="708c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="708c6-103">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="708c6-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="708c6-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="708c6-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="708c6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="708c6-105">Properties</span></span>
|<span data-ttu-id="708c6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="708c6-106">Property</span></span>|<span data-ttu-id="708c6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="708c6-107">Type</span></span>|<span data-ttu-id="708c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="708c6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708c6-109">actionName</span><span class="sxs-lookup"><span data-stu-id="708c6-109">actionName</span></span>|<span data-ttu-id="708c6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="708c6-110">String</span></span>|<span data-ttu-id="708c6-111">Nome da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="708c6-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="708c6-112">actionState</span><span class="sxs-lookup"><span data-stu-id="708c6-112">actionState</span></span>|[<span data-ttu-id="708c6-113">actionState</span><span class="sxs-lookup"><span data-stu-id="708c6-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="708c6-p101">Estado da ação herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="708c6-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="708c6-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="708c6-116">startDateTime</span></span>|<span data-ttu-id="708c6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="708c6-117">DateTimeOffset</span></span>|<span data-ttu-id="708c6-118">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="708c6-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="708c6-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="708c6-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="708c6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="708c6-120">DateTimeOffset</span></span>|<span data-ttu-id="708c6-121">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="708c6-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="708c6-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="708c6-122">userPrincipalName</span></span>|<span data-ttu-id="708c6-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="708c6-123">String</span></span>|<span data-ttu-id="708c6-124">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="708c6-124">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="708c6-125">Relações</span><span class="sxs-lookup"><span data-stu-id="708c6-125">Relationships</span></span>
<span data-ttu-id="708c6-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="708c6-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="708c6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="708c6-127">JSON Representation</span></span>
<span data-ttu-id="708c6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="708c6-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








