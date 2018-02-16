# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="8fc4a-101">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8fc4a-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="8fc4a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8fc4a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fc4a-103">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="8fc4a-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="8fc4a-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8fc4a-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8fc4a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fc4a-105">Properties</span></span>
|<span data-ttu-id="8fc4a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fc4a-106">Property</span></span>|<span data-ttu-id="8fc4a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fc4a-107">Type</span></span>|<span data-ttu-id="8fc4a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fc4a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc4a-109">actionName</span><span class="sxs-lookup"><span data-stu-id="8fc4a-109">actionName</span></span>|<span data-ttu-id="8fc4a-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fc4a-110">String</span></span>|<span data-ttu-id="8fc4a-111">Nome da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8fc4a-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8fc4a-112">actionState</span><span class="sxs-lookup"><span data-stu-id="8fc4a-112">actionState</span></span>|<span data-ttu-id="8fc4a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fc4a-113">String</span></span>|<span data-ttu-id="8fc4a-114">Estado da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8fc4a-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8fc4a-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8fc4a-115">startDateTime</span></span>|<span data-ttu-id="8fc4a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fc4a-116">DateTimeOffset</span></span>|<span data-ttu-id="8fc4a-117">Hora de início da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8fc4a-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8fc4a-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fc4a-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="8fc4a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fc4a-119">DateTimeOffset</span></span>|<span data-ttu-id="8fc4a-120">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8fc4a-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8fc4a-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8fc4a-121">userPrincipalName</span></span>|<span data-ttu-id="8fc4a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fc4a-122">String</span></span>|<span data-ttu-id="8fc4a-123">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="8fc4a-123">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fc4a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="8fc4a-124">Relationships</span></span>
<span data-ttu-id="8fc4a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fc4a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fc4a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fc4a-126">JSON Representation</span></span>
<span data-ttu-id="8fc4a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8fc4a-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
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



