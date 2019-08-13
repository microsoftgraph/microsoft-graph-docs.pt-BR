---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2a971b4e03da4dfdac6dfcdf621715db3e3d1e1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374033"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="331e6-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="331e6-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="331e6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="331e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="331e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="331e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="331e6-107">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="331e6-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="331e6-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="331e6-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="331e6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="331e6-109">Methods</span></span>
|<span data-ttu-id="331e6-110">Método</span><span class="sxs-lookup"><span data-stu-id="331e6-110">Method</span></span>|<span data-ttu-id="331e6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="331e6-111">Return Type</span></span>|<span data-ttu-id="331e6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="331e6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="331e6-113">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="331e6-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="331e6-114">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="331e6-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="331e6-115">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="331e6-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="331e6-116">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="331e6-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="331e6-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="331e6-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="331e6-118">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="331e6-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="331e6-119">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="331e6-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="331e6-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="331e6-120">String collection</span></span>|<span data-ttu-id="331e6-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="331e6-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="331e6-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="331e6-122">Properties</span></span>
|<span data-ttu-id="331e6-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="331e6-123">Property</span></span>|<span data-ttu-id="331e6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="331e6-124">Type</span></span>|<span data-ttu-id="331e6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="331e6-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="331e6-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="331e6-126">createdDateTime</span></span>|<span data-ttu-id="331e6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="331e6-127">DateTimeOffset</span></span>|<span data-ttu-id="331e6-128">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="331e6-128">Date and time of creation</span></span>|
|<span data-ttu-id="331e6-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="331e6-129">lastSyncDateTime</span></span>|<span data-ttu-id="331e6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="331e6-130">DateTimeOffset</span></span>|<span data-ttu-id="331e6-131">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="331e6-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="331e6-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="331e6-132">applicationVersion</span></span>|<span data-ttu-id="331e6-133">String</span><span class="sxs-lookup"><span data-stu-id="331e6-133">String</span></span>|<span data-ttu-id="331e6-134">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="331e6-134">App version</span></span>|
|<span data-ttu-id="331e6-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="331e6-135">managementSdkVersion</span></span>|<span data-ttu-id="331e6-136">String</span><span class="sxs-lookup"><span data-stu-id="331e6-136">String</span></span>|<span data-ttu-id="331e6-137">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="331e6-137">App management SDK version</span></span>|
|<span data-ttu-id="331e6-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="331e6-138">platformVersion</span></span>|<span data-ttu-id="331e6-139">String</span><span class="sxs-lookup"><span data-stu-id="331e6-139">String</span></span>|<span data-ttu-id="331e6-140">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="331e6-140">Operating System version</span></span>|
|<span data-ttu-id="331e6-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="331e6-141">deviceType</span></span>|<span data-ttu-id="331e6-142">String</span><span class="sxs-lookup"><span data-stu-id="331e6-142">String</span></span>|<span data-ttu-id="331e6-143">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="331e6-143">Host device type</span></span>|
|<span data-ttu-id="331e6-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="331e6-144">deviceTag</span></span>|<span data-ttu-id="331e6-145">String</span><span class="sxs-lookup"><span data-stu-id="331e6-145">String</span></span>|<span data-ttu-id="331e6-146">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="331e6-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="331e6-147">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="331e6-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="331e6-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="331e6-148">deviceName</span></span>|<span data-ttu-id="331e6-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="331e6-149">String</span></span>|<span data-ttu-id="331e6-150">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="331e6-150">Host device name</span></span>|
|<span data-ttu-id="331e6-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="331e6-151">managedDeviceId</span></span>|<span data-ttu-id="331e6-152">String</span><span class="sxs-lookup"><span data-stu-id="331e6-152">String</span></span>|<span data-ttu-id="331e6-153">O identificador de dispositivo gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="331e6-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="331e6-154">O valor pode ser vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="331e6-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="331e6-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="331e6-155">azureADDeviceId</span></span>|<span data-ttu-id="331e6-156">String</span><span class="sxs-lookup"><span data-stu-id="331e6-156">String</span></span>|<span data-ttu-id="331e6-157">O identificador de dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="331e6-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="331e6-158">O valor pode ser vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="331e6-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="331e6-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="331e6-159">deviceModel</span></span>|<span data-ttu-id="331e6-160">String</span><span class="sxs-lookup"><span data-stu-id="331e6-160">String</span></span>|<span data-ttu-id="331e6-161">O modelo de dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="331e6-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="331e6-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="331e6-162">deviceManufacturer</span></span>|<span data-ttu-id="331e6-163">String</span><span class="sxs-lookup"><span data-stu-id="331e6-163">String</span></span>|<span data-ttu-id="331e6-164">O fabricante do dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="331e6-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="331e6-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="331e6-165">flaggedReasons</span></span>|<span data-ttu-id="331e6-166">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="331e6-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="331e6-167">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="331e6-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="331e6-168">E.g.</span><span class="sxs-lookup"><span data-stu-id="331e6-168">E.g.</span></span> <span data-ttu-id="331e6-169">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="331e6-169">app running on rooted device</span></span>|
|<span data-ttu-id="331e6-170">userId</span><span class="sxs-lookup"><span data-stu-id="331e6-170">userId</span></span>|<span data-ttu-id="331e6-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="331e6-171">String</span></span>|<span data-ttu-id="331e6-172">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="331e6-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="331e6-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="331e6-173">appIdentifier</span></span>|[<span data-ttu-id="331e6-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="331e6-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="331e6-175">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="331e6-175">The app package Identifier</span></span>|
|<span data-ttu-id="331e6-176">id</span><span class="sxs-lookup"><span data-stu-id="331e6-176">id</span></span>|<span data-ttu-id="331e6-177">String</span><span class="sxs-lookup"><span data-stu-id="331e6-177">String</span></span>|<span data-ttu-id="331e6-178">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="331e6-178">Key of the entity.</span></span>|
|<span data-ttu-id="331e6-179">versão</span><span class="sxs-lookup"><span data-stu-id="331e6-179">version</span></span>|<span data-ttu-id="331e6-180">String</span><span class="sxs-lookup"><span data-stu-id="331e6-180">String</span></span>|<span data-ttu-id="331e6-181">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="331e6-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="331e6-182">Relações</span><span class="sxs-lookup"><span data-stu-id="331e6-182">Relationships</span></span>
|<span data-ttu-id="331e6-183">Relação</span><span class="sxs-lookup"><span data-stu-id="331e6-183">Relationship</span></span>|<span data-ttu-id="331e6-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="331e6-184">Type</span></span>|<span data-ttu-id="331e6-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="331e6-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="331e6-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="331e6-186">appliedPolicies</span></span>|<span data-ttu-id="331e6-187">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="331e6-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="331e6-188">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="331e6-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="331e6-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="331e6-189">intendedPolicies</span></span>|<span data-ttu-id="331e6-190">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="331e6-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="331e6-191">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="331e6-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="331e6-192">operations</span><span class="sxs-lookup"><span data-stu-id="331e6-192">operations</span></span>|<span data-ttu-id="331e6-193">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="331e6-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="331e6-194">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="331e6-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="331e6-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="331e6-195">JSON Representation</span></span>
<span data-ttu-id="331e6-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="331e6-196">Here is a JSON representation of the resource.</span></span>
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



