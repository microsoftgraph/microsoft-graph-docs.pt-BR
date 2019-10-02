---
title: Tipo de recurso de usuário
description: Representa um objeto de usuário do Azure Active Directory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 15fca0cedc6fe1da81da25688bbc447c1f8f475f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360101"
---
# <a name="user-resource-type"></a><span data-ttu-id="e1b77-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="e1b77-103">user resource type</span></span>

> <span data-ttu-id="e1b77-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b77-105">Representa um objeto de usuário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1b77-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="e1b77-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1b77-106">Methods</span></span>
|<span data-ttu-id="e1b77-107">Método</span><span class="sxs-lookup"><span data-stu-id="e1b77-107">Method</span></span>|<span data-ttu-id="e1b77-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1b77-108">Return Type</span></span>|<span data-ttu-id="e1b77-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b77-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b77-110">[Listar objetos Users](../api/intune-shared-user-list.md) .</span><span class="sxs-lookup"><span data-stu-id="e1b77-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="e1b77-111">Conjunto [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="e1b77-112">Listar propriedades e relações de objetos de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="e1b77-113">[Obtenha](../api/intune-shared-user-get.md) o objeto user.</span><span class="sxs-lookup"><span data-stu-id="e1b77-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="e1b77-114">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="e1b77-115">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="e1b77-116">[Criar objeto user](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="e1b77-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="e1b77-117">Coleção [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="e1b77-118">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="e1b77-119">[Excluir usuário](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="e1b77-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1b77-120">None</span></span>|<span data-ttu-id="e1b77-121">Excluir [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="e1b77-122">[Atualize](../api/intune-shared-user-update.md) o objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="e1b77-123">user</span><span class="sxs-lookup"><span data-stu-id="e1b77-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="e1b77-124">Atualizar as propriedades de um objeto de [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b77-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="e1b77-125">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="e1b77-125">**Device management**</span></span>|
|[<span data-ttu-id="e1b77-126">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="e1b77-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="e1b77-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1b77-127">None</span></span>|<span data-ttu-id="e1b77-128">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="e1b77-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="e1b77-129">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="e1b77-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="e1b77-130">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="e1b77-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="e1b77-131">Conjunto [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="e1b77-132">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="e1b77-133">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="e1b77-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="e1b77-134">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e1b77-135">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="e1b77-136">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="e1b77-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="e1b77-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1b77-137">None</span></span>|<span data-ttu-id="e1b77-138">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="e1b77-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1b77-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1b77-139">Properties</span></span>
|<span data-ttu-id="e1b77-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1b77-140">Property</span></span>|<span data-ttu-id="e1b77-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1b77-141">Type</span></span>|<span data-ttu-id="e1b77-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b77-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b77-143">id</span><span class="sxs-lookup"><span data-stu-id="e1b77-143">id</span></span>|<span data-ttu-id="e1b77-144">String</span><span class="sxs-lookup"><span data-stu-id="e1b77-144">String</span></span>|<span data-ttu-id="e1b77-145">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="e1b77-146">**Integração**</span><span class="sxs-lookup"><span data-stu-id="e1b77-146">**Onboarding**</span></span>|
|<span data-ttu-id="e1b77-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="e1b77-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="e1b77-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b77-148">Int32</span></span>|<span data-ttu-id="e1b77-149">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="e1b77-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="e1b77-150">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="e1b77-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e1b77-151">Relações</span><span class="sxs-lookup"><span data-stu-id="e1b77-151">Relationships</span></span>
|<span data-ttu-id="e1b77-152">Relação</span><span class="sxs-lookup"><span data-stu-id="e1b77-152">Relationship</span></span>|<span data-ttu-id="e1b77-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1b77-153">Type</span></span>|<span data-ttu-id="e1b77-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b77-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b77-155">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="e1b77-155">**Device management**</span></span>|
|<span data-ttu-id="e1b77-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="e1b77-156">managedDevices</span></span>|<span data-ttu-id="e1b77-157">Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="e1b77-158">Os dispositivos gerenciados associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="e1b77-159">**Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="e1b77-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="e1b77-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="e1b77-160">managedAppRegistrations</span></span>|<span data-ttu-id="e1b77-161">Conjunto [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="e1b77-162">Zero ou mais registros de aplicativos gerenciados que pertencem ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="e1b77-163">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="e1b77-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="e1b77-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="e1b77-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="e1b77-165">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e1b77-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="e1b77-166">A lista de eventos de solução de problemas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="e1b77-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1b77-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1b77-167">JSON Representation</span></span>
<span data-ttu-id="e1b77-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1b77-168">Here is a JSON representation of the resource.</span></span>
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

