---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f486e3202535882d719e5f6c083b583321e917b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020570"
---
# <a name="user-resource-type"></a><span data-ttu-id="998a0-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="998a0-103">user resource type</span></span>

<span data-ttu-id="998a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="998a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="998a0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="998a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="998a0-106">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="998a0-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="998a0-107">Methods</span><span class="sxs-lookup"><span data-stu-id="998a0-107">Methods</span></span>
|<span data-ttu-id="998a0-108">Método</span><span class="sxs-lookup"><span data-stu-id="998a0-108">Method</span></span>|<span data-ttu-id="998a0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="998a0-109">Return Type</span></span>|<span data-ttu-id="998a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="998a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998a0-111">[Listar objetos Users](../api/intune-shared-user-list.md) .</span><span class="sxs-lookup"><span data-stu-id="998a0-111">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="998a0-112">Conjunto [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-112">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="998a0-113">Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-113">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="998a0-114">[Obtenha](../api/intune-shared-user-get.md) o objeto user.</span><span class="sxs-lookup"><span data-stu-id="998a0-114">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="998a0-115">Coleção [usuário](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-115">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="998a0-116">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-116">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="998a0-117">[Criar objeto user](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="998a0-117">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="998a0-118">Coleção [usuário](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-118">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="998a0-119">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-119">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="998a0-120">[Excluir usuário](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-120">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="998a0-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="998a0-121">None</span></span>|<span data-ttu-id="998a0-122">Excluir [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-122">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="998a0-123">[Atualize](../api/intune-shared-user-update.md) o objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-123">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="998a0-124">user</span><span class="sxs-lookup"><span data-stu-id="998a0-124">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="998a0-125">Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="998a0-125">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="998a0-126">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="998a0-126">**Device management**</span></span>|
|[<span data-ttu-id="998a0-127">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="998a0-127">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="998a0-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="998a0-128">None</span></span>|<span data-ttu-id="998a0-129">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="998a0-129">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="998a0-130">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="998a0-130">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="998a0-131">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="998a0-131">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="998a0-132">Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-132">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="998a0-133">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-133">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="998a0-134">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="998a0-134">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="998a0-135">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="998a0-136">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-136">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="998a0-137">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="998a0-137">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="998a0-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="998a0-138">None</span></span>|<span data-ttu-id="998a0-139">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="998a0-139">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="998a0-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="998a0-140">Properties</span></span>
|<span data-ttu-id="998a0-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="998a0-141">Property</span></span>|<span data-ttu-id="998a0-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="998a0-142">Type</span></span>|<span data-ttu-id="998a0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="998a0-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998a0-144">id</span><span class="sxs-lookup"><span data-stu-id="998a0-144">id</span></span>|<span data-ttu-id="998a0-145">String</span><span class="sxs-lookup"><span data-stu-id="998a0-145">String</span></span>|<span data-ttu-id="998a0-146">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-146">Unique identifier of the user.</span></span>|
|<span data-ttu-id="998a0-147">**Integração**</span><span class="sxs-lookup"><span data-stu-id="998a0-147">**Onboarding**</span></span>|
|<span data-ttu-id="998a0-148">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="998a0-148">deviceEnrollmentLimit</span></span>|<span data-ttu-id="998a0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="998a0-149">Int32</span></span>|<span data-ttu-id="998a0-150">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="998a0-150">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="998a0-151">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="998a0-151">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="998a0-152">Relações</span><span class="sxs-lookup"><span data-stu-id="998a0-152">Relationships</span></span>
|<span data-ttu-id="998a0-153">Relação</span><span class="sxs-lookup"><span data-stu-id="998a0-153">Relationship</span></span>|<span data-ttu-id="998a0-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="998a0-154">Type</span></span>|<span data-ttu-id="998a0-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="998a0-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="998a0-156">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="998a0-156">**Device management**</span></span>|
|<span data-ttu-id="998a0-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="998a0-157">managedDevices</span></span>|<span data-ttu-id="998a0-158">Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="998a0-159">Os dispositivos gerenciados associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-159">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="998a0-160">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="998a0-160">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="998a0-161">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="998a0-161">managedAppRegistrations</span></span>|<span data-ttu-id="998a0-162">Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="998a0-163">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-163">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="998a0-164">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="998a0-164">**Troubleshooting**</span></span>|
|<span data-ttu-id="998a0-165">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="998a0-165">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="998a0-166">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="998a0-166">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="998a0-167">A lista de eventos de solução de problemas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="998a0-167">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="998a0-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="998a0-168">JSON Representation</span></span>
<span data-ttu-id="998a0-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="998a0-169">Here is a JSON representation of the resource.</span></span>
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






