---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
ms.openlocfilehash: 5d1d8e18e120fb26cfd5cea1cd223a6c38ad0aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006080"
---
# <a name="user-resource-type"></a><span data-ttu-id="88d6a-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="88d6a-103">user resource type</span></span>

> <span data-ttu-id="88d6a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="88d6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88d6a-105">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="88d6a-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="88d6a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="88d6a-106">Methods</span></span>
|<span data-ttu-id="88d6a-107">Método</span><span class="sxs-lookup"><span data-stu-id="88d6a-107">Method</span></span>|<span data-ttu-id="88d6a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88d6a-108">Return Type</span></span>|<span data-ttu-id="88d6a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d6a-110">[Os usuários da lista](../api/intune-shared-user-list.md) de objetos.</span><span class="sxs-lookup"><span data-stu-id="88d6a-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="88d6a-111">Conjunto [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="88d6a-112">Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="88d6a-113">Objeto [obter do usuário](../api/intune-shared-user-get.md) .</span><span class="sxs-lookup"><span data-stu-id="88d6a-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="88d6a-114">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="88d6a-115">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="88d6a-116">Objeto de [usuário de criar](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="88d6a-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="88d6a-117">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="88d6a-118">Criar um novo objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="88d6a-119">[Excluir o usuário](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="88d6a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88d6a-120">None</span></span>|<span data-ttu-id="88d6a-121">Excluir [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="88d6a-122">Objeto de [usuário de atualização](../api/intune-shared-user-update.md) .</span><span class="sxs-lookup"><span data-stu-id="88d6a-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="88d6a-123">user</span><span class="sxs-lookup"><span data-stu-id="88d6a-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="88d6a-124">Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="88d6a-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="88d6a-125">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="88d6a-125">**Device management**</span></span>|
|[<span data-ttu-id="88d6a-126">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="88d6a-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="88d6a-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88d6a-127">None</span></span>|<span data-ttu-id="88d6a-128">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="88d6a-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="88d6a-129">**Gerenciamento de aplicativo móvel (MAM)**</span><span class="sxs-lookup"><span data-stu-id="88d6a-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="88d6a-130">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="88d6a-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="88d6a-131">Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="88d6a-132">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="88d6a-133">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="88d6a-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="88d6a-134">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="88d6a-135">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="88d6a-136">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="88d6a-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="88d6a-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88d6a-137">None</span></span>|<span data-ttu-id="88d6a-138">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="88d6a-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="88d6a-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88d6a-139">Properties</span></span>
|<span data-ttu-id="88d6a-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88d6a-140">Property</span></span>|<span data-ttu-id="88d6a-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="88d6a-141">Type</span></span>|<span data-ttu-id="88d6a-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d6a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d6a-143">id</span><span class="sxs-lookup"><span data-stu-id="88d6a-143">id</span></span>|<span data-ttu-id="88d6a-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88d6a-144">String</span></span>|<span data-ttu-id="88d6a-145">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="88d6a-146">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="88d6a-146">**Onboarding**</span></span>|
|<span data-ttu-id="88d6a-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="88d6a-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="88d6a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="88d6a-148">Int32</span></span>|<span data-ttu-id="88d6a-149">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="88d6a-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="88d6a-150">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="88d6a-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="88d6a-151">Relações</span><span class="sxs-lookup"><span data-stu-id="88d6a-151">Relationships</span></span>
|<span data-ttu-id="88d6a-152">Relação</span><span class="sxs-lookup"><span data-stu-id="88d6a-152">Relationship</span></span>|<span data-ttu-id="88d6a-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="88d6a-153">Type</span></span>|<span data-ttu-id="88d6a-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d6a-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d6a-155">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="88d6a-155">**Device management**</span></span>|
|<span data-ttu-id="88d6a-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="88d6a-156">managedDevices</span></span>|<span data-ttu-id="88d6a-157">Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="88d6a-158">Os dispositivos gerenciados associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="88d6a-159">**Gerenciamento de aplicativo móvel (MAM)**</span><span class="sxs-lookup"><span data-stu-id="88d6a-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="88d6a-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="88d6a-160">managedAppRegistrations</span></span>|<span data-ttu-id="88d6a-161">Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="88d6a-162">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="88d6a-163">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="88d6a-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="88d6a-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="88d6a-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="88d6a-165">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="88d6a-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="88d6a-166">A lista de eventos de solução de problemas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="88d6a-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88d6a-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88d6a-167">JSON Representation</span></span>
<span data-ttu-id="88d6a-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88d6a-168">Here is a JSON representation of the resource.</span></span>
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
