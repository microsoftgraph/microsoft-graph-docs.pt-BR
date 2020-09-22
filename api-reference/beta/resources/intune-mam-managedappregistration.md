---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c2ea9eaf64a4d198ca37fa7c485ee6817c9d749
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030196"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="7f806-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="7f806-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="7f806-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f806-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f806-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f806-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f806-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f806-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f806-108">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7f806-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="7f806-109">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="7f806-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7f806-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f806-110">Methods</span></span>
|<span data-ttu-id="7f806-111">Método</span><span class="sxs-lookup"><span data-stu-id="7f806-111">Method</span></span>|<span data-ttu-id="7f806-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f806-112">Return Type</span></span>|<span data-ttu-id="7f806-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f806-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f806-114">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="7f806-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="7f806-115">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="7f806-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="7f806-116">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="7f806-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="7f806-117">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="7f806-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="7f806-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="7f806-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="7f806-119">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="7f806-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="7f806-120">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="7f806-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="7f806-121">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7f806-121">String collection</span></span>|<span data-ttu-id="7f806-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7f806-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7f806-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f806-123">Properties</span></span>
|<span data-ttu-id="7f806-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f806-124">Property</span></span>|<span data-ttu-id="7f806-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f806-125">Type</span></span>|<span data-ttu-id="7f806-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f806-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f806-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f806-127">createdDateTime</span></span>|<span data-ttu-id="7f806-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f806-128">DateTimeOffset</span></span>|<span data-ttu-id="7f806-129">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="7f806-129">Date and time of creation</span></span>|
|<span data-ttu-id="7f806-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7f806-130">lastSyncDateTime</span></span>|<span data-ttu-id="7f806-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f806-131">DateTimeOffset</span></span>|<span data-ttu-id="7f806-132">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7f806-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="7f806-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="7f806-133">applicationVersion</span></span>|<span data-ttu-id="7f806-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-134">String</span></span>|<span data-ttu-id="7f806-135">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f806-135">App version</span></span>|
|<span data-ttu-id="7f806-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="7f806-136">managementSdkVersion</span></span>|<span data-ttu-id="7f806-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-137">String</span></span>|<span data-ttu-id="7f806-138">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f806-138">App management SDK version</span></span>|
|<span data-ttu-id="7f806-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="7f806-139">platformVersion</span></span>|<span data-ttu-id="7f806-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-140">String</span></span>|<span data-ttu-id="7f806-141">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7f806-141">Operating System version</span></span>|
|<span data-ttu-id="7f806-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="7f806-142">deviceType</span></span>|<span data-ttu-id="7f806-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-143">String</span></span>|<span data-ttu-id="7f806-144">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="7f806-144">Host device type</span></span>|
|<span data-ttu-id="7f806-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="7f806-145">deviceTag</span></span>|<span data-ttu-id="7f806-146">String</span><span class="sxs-lookup"><span data-stu-id="7f806-146">String</span></span>|<span data-ttu-id="7f806-147">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f806-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="7f806-148">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="7f806-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="7f806-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="7f806-149">deviceName</span></span>|<span data-ttu-id="7f806-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-150">String</span></span>|<span data-ttu-id="7f806-151">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="7f806-151">Host device name</span></span>|
|<span data-ttu-id="7f806-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7f806-152">managedDeviceId</span></span>|<span data-ttu-id="7f806-153">String</span><span class="sxs-lookup"><span data-stu-id="7f806-153">String</span></span>|<span data-ttu-id="7f806-154">O identificador de dispositivo gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="7f806-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="7f806-155">O valor pode ser vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7f806-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="7f806-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="7f806-156">azureADDeviceId</span></span>|<span data-ttu-id="7f806-157">String</span><span class="sxs-lookup"><span data-stu-id="7f806-157">String</span></span>|<span data-ttu-id="7f806-158">O identificador de dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="7f806-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="7f806-159">O valor pode ser vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7f806-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="7f806-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7f806-160">deviceModel</span></span>|<span data-ttu-id="7f806-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-161">String</span></span>|<span data-ttu-id="7f806-162">O modelo de dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="7f806-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="7f806-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="7f806-163">deviceManufacturer</span></span>|<span data-ttu-id="7f806-164">String</span><span class="sxs-lookup"><span data-stu-id="7f806-164">String</span></span>|<span data-ttu-id="7f806-165">O fabricante do dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="7f806-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="7f806-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="7f806-166">flaggedReasons</span></span>|<span data-ttu-id="7f806-167">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="7f806-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="7f806-168">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f806-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="7f806-169">E.g.</span><span class="sxs-lookup"><span data-stu-id="7f806-169">E.g.</span></span> <span data-ttu-id="7f806-170">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="7f806-170">app running on rooted device</span></span>|
|<span data-ttu-id="7f806-171">userId</span><span class="sxs-lookup"><span data-stu-id="7f806-171">userId</span></span>|<span data-ttu-id="7f806-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f806-172">String</span></span>|<span data-ttu-id="7f806-173">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="7f806-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="7f806-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f806-174">appIdentifier</span></span>|[<span data-ttu-id="7f806-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f806-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="7f806-176">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f806-176">The app package Identifier</span></span>|
|<span data-ttu-id="7f806-177">id</span><span class="sxs-lookup"><span data-stu-id="7f806-177">id</span></span>|<span data-ttu-id="7f806-178">String</span><span class="sxs-lookup"><span data-stu-id="7f806-178">String</span></span>|<span data-ttu-id="7f806-179">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f806-179">Key of the entity.</span></span>|
|<span data-ttu-id="7f806-180">versão</span><span class="sxs-lookup"><span data-stu-id="7f806-180">version</span></span>|<span data-ttu-id="7f806-181">String</span><span class="sxs-lookup"><span data-stu-id="7f806-181">String</span></span>|<span data-ttu-id="7f806-182">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f806-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f806-183">Relações</span><span class="sxs-lookup"><span data-stu-id="7f806-183">Relationships</span></span>
|<span data-ttu-id="7f806-184">Relação</span><span class="sxs-lookup"><span data-stu-id="7f806-184">Relationship</span></span>|<span data-ttu-id="7f806-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f806-185">Type</span></span>|<span data-ttu-id="7f806-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f806-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f806-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="7f806-187">appliedPolicies</span></span>|<span data-ttu-id="7f806-188">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f806-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="7f806-189">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7f806-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="7f806-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="7f806-190">intendedPolicies</span></span>|<span data-ttu-id="7f806-191">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f806-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="7f806-192">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="7f806-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="7f806-193">operations</span><span class="sxs-lookup"><span data-stu-id="7f806-193">operations</span></span>|<span data-ttu-id="7f806-194">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="7f806-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="7f806-195">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f806-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f806-196">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f806-196">JSON Representation</span></span>
<span data-ttu-id="7f806-197">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f806-197">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```






