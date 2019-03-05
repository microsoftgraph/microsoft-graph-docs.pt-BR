---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7a6c87b5c073e00b660db807ff38c454c302d94
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253404"
---
# <a name="user-resource-type"></a><span data-ttu-id="6dc64-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="6dc64-103">user resource type</span></span>

> <span data-ttu-id="6dc64-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc64-105">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6dc64-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="6dc64-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6dc64-106">Methods</span></span>
|<span data-ttu-id="6dc64-107">Método</span><span class="sxs-lookup"><span data-stu-id="6dc64-107">Method</span></span>|<span data-ttu-id="6dc64-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6dc64-108">Return Type</span></span>|<span data-ttu-id="6dc64-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc64-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc64-110">[Listar](../api/intune-shared-user-list.md) objetos users.</span><span class="sxs-lookup"><span data-stu-id="6dc64-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="6dc64-111">Conjunto [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="6dc64-112">Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="6dc64-113">[Obtenha](../api/intune-shared-user-get.md) o objeto user.</span><span class="sxs-lookup"><span data-stu-id="6dc64-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="6dc64-114">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="6dc64-115">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="6dc64-116">[Criar objeto user](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc64-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="6dc64-117">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="6dc64-118">Criar um novo objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="6dc64-119">[Excluir usuário](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="6dc64-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dc64-120">None</span></span>|<span data-ttu-id="6dc64-121">Excluir [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="6dc64-122">[Atualize](../api/intune-shared-user-update.md) o objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="6dc64-123">user</span><span class="sxs-lookup"><span data-stu-id="6dc64-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="6dc64-124">Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6dc64-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="6dc64-125">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="6dc64-125">**Device management**</span></span>|
|[<span data-ttu-id="6dc64-126">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="6dc64-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="6dc64-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dc64-127">None</span></span>|<span data-ttu-id="6dc64-128">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="6dc64-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="6dc64-129">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="6dc64-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="6dc64-130">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="6dc64-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="6dc64-131">Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="6dc64-132">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="6dc64-133">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="6dc64-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="6dc64-134">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6dc64-135">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="6dc64-136">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="6dc64-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="6dc64-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dc64-137">None</span></span>|<span data-ttu-id="6dc64-138">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="6dc64-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="6dc64-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dc64-139">Properties</span></span>
|<span data-ttu-id="6dc64-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dc64-140">Property</span></span>|<span data-ttu-id="6dc64-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc64-141">Type</span></span>|<span data-ttu-id="6dc64-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc64-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc64-143">id</span><span class="sxs-lookup"><span data-stu-id="6dc64-143">id</span></span>|<span data-ttu-id="6dc64-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dc64-144">String</span></span>|<span data-ttu-id="6dc64-145">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="6dc64-146">**Integração**</span><span class="sxs-lookup"><span data-stu-id="6dc64-146">**Onboarding**</span></span>|
|<span data-ttu-id="6dc64-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="6dc64-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="6dc64-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6dc64-148">Int32</span></span>|<span data-ttu-id="6dc64-149">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="6dc64-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="6dc64-150">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="6dc64-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6dc64-151">Relações</span><span class="sxs-lookup"><span data-stu-id="6dc64-151">Relationships</span></span>
|<span data-ttu-id="6dc64-152">Relação</span><span class="sxs-lookup"><span data-stu-id="6dc64-152">Relationship</span></span>|<span data-ttu-id="6dc64-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc64-153">Type</span></span>|<span data-ttu-id="6dc64-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc64-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc64-155">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="6dc64-155">**Device management**</span></span>|
|<span data-ttu-id="6dc64-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="6dc64-156">managedDevices</span></span>|<span data-ttu-id="6dc64-157">Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="6dc64-158">Os dispositivos gerenciados associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="6dc64-159">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="6dc64-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="6dc64-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6dc64-160">managedAppRegistrations</span></span>|<span data-ttu-id="6dc64-161">Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="6dc64-162">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="6dc64-163">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="6dc64-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="6dc64-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="6dc64-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="6dc64-165">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="6dc64-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="6dc64-166">A lista de eventos de solução de problemas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc64-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dc64-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dc64-167">JSON Representation</span></span>
<span data-ttu-id="6dc64-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dc64-168">Here is a JSON representation of the resource.</span></span>
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
