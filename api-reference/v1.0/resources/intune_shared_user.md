# <a name="user-resource-type"></a><span data-ttu-id="68c19-101">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="68c19-101">user resource type</span></span>

> <span data-ttu-id="68c19-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="68c19-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68c19-103">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="68c19-103">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="68c19-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="68c19-104">Methods</span></span>
|<span data-ttu-id="68c19-105">Método</span><span class="sxs-lookup"><span data-stu-id="68c19-105">Method</span></span>|<span data-ttu-id="68c19-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68c19-106">Return Type</span></span>|<span data-ttu-id="68c19-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c19-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c19-108">Objetos [List users](../api/intune_shared_user_list.md).</span><span class="sxs-lookup"><span data-stu-id="68c19-108">[List users](../api/intune_shared_user_list.md) objects.</span></span>|
|<span data-ttu-id="68c19-109">Objeto [Get user](../api/intune_shared_user_get.md).</span><span class="sxs-lookup"><span data-stu-id="68c19-109">[Get user](../api/intune_shared_user_get.md) object.</span></span>|
|<span data-ttu-id="68c19-110">Objeto  [Create user](../api/intune_shared_user_create.md).</span><span class="sxs-lookup"><span data-stu-id="68c19-110">Create a new [user](../api/intune_shared_user_create.md) object.</span></span>|
|<span data-ttu-id="68c19-111">[Delete user](../api/intune_shared_user_delete.md).</span><span class="sxs-lookup"><span data-stu-id="68c19-111">Delete user</span></span>|
|<span data-ttu-id="68c19-112">Objeto [Update user](../api/intune_shared_user_update.md).</span><span class="sxs-lookup"><span data-stu-id="68c19-112">Update user object.</span></span>|
|<span data-ttu-id="68c19-113">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="68c19-113">**Device management**</span></span>|
|[<span data-ttu-id="68c19-114">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="68c19-114">removeAllDevicesFromManagement action</span></span>](../api/intune_shared_user_removealldevicesfrommanagement.md)|<span data-ttu-id="68c19-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68c19-115">None</span></span>|<span data-ttu-id="68c19-116">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="68c19-116">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="68c19-117">**Gerenciamento de aplicativo móvel (MAM)**</span><span class="sxs-lookup"><span data-stu-id="68c19-117">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="68c19-118">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="68c19-118">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="68c19-119">Conjunto [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="68c19-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="68c19-120">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-120">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="68c19-121">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="68c19-121">getManagedAppPolicies function</span></span>](../api/intune_shared_user_getmanagedapppolicies.md)|<span data-ttu-id="68c19-122">Conjunto [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="68c19-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="68c19-123">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-123">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="68c19-124">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="68c19-124">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="68c19-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68c19-125">None</span></span>|<span data-ttu-id="68c19-126">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="68c19-126">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="68c19-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68c19-127">Properties</span></span>
|<span data-ttu-id="68c19-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68c19-128">Property</span></span>|<span data-ttu-id="68c19-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="68c19-129">Type</span></span>|<span data-ttu-id="68c19-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c19-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c19-131">id</span><span class="sxs-lookup"><span data-stu-id="68c19-131">id</span></span>|<span data-ttu-id="68c19-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c19-132">String</span></span>|<span data-ttu-id="68c19-133">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-133">Unique identifier of the user.</span></span>|
|<span data-ttu-id="68c19-134">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="68c19-134">**On-boarding**</span></span>|
|<span data-ttu-id="68c19-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="68c19-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="68c19-136">Int32</span><span class="sxs-lookup"><span data-stu-id="68c19-136">Int32</span></span>|<span data-ttu-id="68c19-137">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="68c19-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="68c19-138">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="68c19-138">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="68c19-139">Relações</span><span class="sxs-lookup"><span data-stu-id="68c19-139">Relationships</span></span>
|<span data-ttu-id="68c19-140">Relação</span><span class="sxs-lookup"><span data-stu-id="68c19-140">Relationship</span></span>|<span data-ttu-id="68c19-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="68c19-141">Type</span></span>|<span data-ttu-id="68c19-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c19-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c19-143">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="68c19-143">**Device management**</span></span>|
|<span data-ttu-id="68c19-144">managedDevices</span><span class="sxs-lookup"><span data-stu-id="68c19-144">managedDevices</span></span>|<span data-ttu-id="68c19-145">Conjunto [managedDevice](../resources/intune_devices_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="68c19-145">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="68c19-146">Os dispositivos gerenciados associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-146">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="68c19-147">**Gerenciamento de aplicativo móvel (MAM)**</span><span class="sxs-lookup"><span data-stu-id="68c19-147">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="68c19-148">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="68c19-148">managedAppRegistrations</span></span>|<span data-ttu-id="68c19-149">Conjunto [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="68c19-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="68c19-150">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-150">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="68c19-151">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="68c19-151">**Troubleshooting**</span></span>|
|<span data-ttu-id="68c19-152">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="68c19-152">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="68c19-153">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="68c19-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="68c19-154">A lista de eventos de solução de problemas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="68c19-154">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68c19-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68c19-155">JSON Representation</span></span>
<span data-ttu-id="68c19-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68c19-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
