---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a909c50e6ac7f40c43f4d573f1966f9bb35a3fa6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371991"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="0bebe-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0bebe-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="0bebe-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bebe-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bebe-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bebe-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bebe-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bebe-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bebe-108">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0bebe-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="0bebe-109">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="0bebe-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0bebe-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0bebe-110">Methods</span></span>
|<span data-ttu-id="0bebe-111">Método</span><span class="sxs-lookup"><span data-stu-id="0bebe-111">Method</span></span>|<span data-ttu-id="0bebe-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0bebe-112">Return Type</span></span>|<span data-ttu-id="0bebe-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bebe-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0bebe-114">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="0bebe-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="0bebe-115">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebe-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="0bebe-116">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0bebe-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="0bebe-117">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="0bebe-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="0bebe-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0bebe-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="0bebe-119">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0bebe-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="0bebe-120">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0bebe-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="0bebe-121">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0bebe-121">String collection</span></span>|<span data-ttu-id="0bebe-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bebe-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0bebe-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bebe-123">Properties</span></span>
|<span data-ttu-id="0bebe-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bebe-124">Property</span></span>|<span data-ttu-id="0bebe-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bebe-125">Type</span></span>|<span data-ttu-id="0bebe-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bebe-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bebe-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bebe-127">createdDateTime</span></span>|<span data-ttu-id="0bebe-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bebe-128">DateTimeOffset</span></span>|<span data-ttu-id="0bebe-129">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="0bebe-129">Date and time of creation</span></span>|
|<span data-ttu-id="0bebe-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0bebe-130">lastSyncDateTime</span></span>|<span data-ttu-id="0bebe-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bebe-131">DateTimeOffset</span></span>|<span data-ttu-id="0bebe-132">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0bebe-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="0bebe-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0bebe-133">applicationVersion</span></span>|<span data-ttu-id="0bebe-134">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-134">String</span></span>|<span data-ttu-id="0bebe-135">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bebe-135">App version</span></span>|
|<span data-ttu-id="0bebe-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0bebe-136">managementSdkVersion</span></span>|<span data-ttu-id="0bebe-137">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-137">String</span></span>|<span data-ttu-id="0bebe-138">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bebe-138">App management SDK version</span></span>|
|<span data-ttu-id="0bebe-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="0bebe-139">platformVersion</span></span>|<span data-ttu-id="0bebe-140">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-140">String</span></span>|<span data-ttu-id="0bebe-141">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="0bebe-141">Operating System version</span></span>|
|<span data-ttu-id="0bebe-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="0bebe-142">deviceType</span></span>|<span data-ttu-id="0bebe-143">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-143">String</span></span>|<span data-ttu-id="0bebe-144">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="0bebe-144">Host device type</span></span>|
|<span data-ttu-id="0bebe-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0bebe-145">deviceTag</span></span>|<span data-ttu-id="0bebe-146">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-146">String</span></span>|<span data-ttu-id="0bebe-147">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bebe-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="0bebe-148">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="0bebe-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="0bebe-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="0bebe-149">deviceName</span></span>|<span data-ttu-id="0bebe-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bebe-150">String</span></span>|<span data-ttu-id="0bebe-151">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="0bebe-151">Host device name</span></span>|
|<span data-ttu-id="0bebe-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0bebe-152">managedDeviceId</span></span>|<span data-ttu-id="0bebe-153">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-153">String</span></span>|<span data-ttu-id="0bebe-154">O identificador de dispositivo gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="0bebe-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="0bebe-155">O valor pode ser vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0bebe-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="0bebe-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0bebe-156">azureADDeviceId</span></span>|<span data-ttu-id="0bebe-157">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-157">String</span></span>|<span data-ttu-id="0bebe-158">O identificador de dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="0bebe-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="0bebe-159">O valor pode ser vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bebe-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0bebe-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0bebe-160">deviceModel</span></span>|<span data-ttu-id="0bebe-161">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-161">String</span></span>|<span data-ttu-id="0bebe-162">O modelo de dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="0bebe-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="0bebe-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="0bebe-163">deviceManufacturer</span></span>|<span data-ttu-id="0bebe-164">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-164">String</span></span>|<span data-ttu-id="0bebe-165">O fabricante do dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="0bebe-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="0bebe-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="0bebe-166">flaggedReasons</span></span>|<span data-ttu-id="0bebe-167">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="0bebe-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="0bebe-168">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bebe-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="0bebe-169">E.g.</span><span class="sxs-lookup"><span data-stu-id="0bebe-169">E.g.</span></span> <span data-ttu-id="0bebe-170">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="0bebe-170">app running on rooted device</span></span>|
|<span data-ttu-id="0bebe-171">userId</span><span class="sxs-lookup"><span data-stu-id="0bebe-171">userId</span></span>|<span data-ttu-id="0bebe-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bebe-172">String</span></span>|<span data-ttu-id="0bebe-173">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="0bebe-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="0bebe-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0bebe-174">appIdentifier</span></span>|[<span data-ttu-id="0bebe-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0bebe-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="0bebe-176">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bebe-176">The app package Identifier</span></span>|
|<span data-ttu-id="0bebe-177">id</span><span class="sxs-lookup"><span data-stu-id="0bebe-177">id</span></span>|<span data-ttu-id="0bebe-178">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-178">String</span></span>|<span data-ttu-id="0bebe-179">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bebe-179">Key of the entity.</span></span>|
|<span data-ttu-id="0bebe-180">versão</span><span class="sxs-lookup"><span data-stu-id="0bebe-180">version</span></span>|<span data-ttu-id="0bebe-181">String</span><span class="sxs-lookup"><span data-stu-id="0bebe-181">String</span></span>|<span data-ttu-id="0bebe-182">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bebe-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bebe-183">Relações</span><span class="sxs-lookup"><span data-stu-id="0bebe-183">Relationships</span></span>
|<span data-ttu-id="0bebe-184">Relação</span><span class="sxs-lookup"><span data-stu-id="0bebe-184">Relationship</span></span>|<span data-ttu-id="0bebe-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bebe-185">Type</span></span>|<span data-ttu-id="0bebe-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bebe-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bebe-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="0bebe-187">appliedPolicies</span></span>|<span data-ttu-id="0bebe-188">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0bebe-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0bebe-189">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0bebe-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="0bebe-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="0bebe-190">intendedPolicies</span></span>|<span data-ttu-id="0bebe-191">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0bebe-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0bebe-192">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="0bebe-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="0bebe-193">operations</span><span class="sxs-lookup"><span data-stu-id="0bebe-193">operations</span></span>|<span data-ttu-id="0bebe-194">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0bebe-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="0bebe-195">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bebe-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bebe-196">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bebe-196">JSON Representation</span></span>
<span data-ttu-id="0bebe-197">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bebe-197">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



