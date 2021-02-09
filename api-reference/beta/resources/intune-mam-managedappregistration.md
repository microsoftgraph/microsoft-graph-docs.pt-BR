---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7c762c2477439010562c0e7e1b7ddf565d3203e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157558"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="0191f-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0191f-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="0191f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0191f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0191f-106">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0191f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0191f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0191f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0191f-108">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0191f-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="0191f-109">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="0191f-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0191f-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0191f-110">Methods</span></span>
|<span data-ttu-id="0191f-111">Método</span><span class="sxs-lookup"><span data-stu-id="0191f-111">Method</span></span>|<span data-ttu-id="0191f-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0191f-112">Return Type</span></span>|<span data-ttu-id="0191f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0191f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0191f-114">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="0191f-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="0191f-115">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="0191f-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="0191f-116">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0191f-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="0191f-117">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="0191f-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="0191f-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0191f-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="0191f-119">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0191f-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="0191f-120">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0191f-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="0191f-121">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0191f-121">String collection</span></span>|<span data-ttu-id="0191f-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0191f-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0191f-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0191f-123">Properties</span></span>
|<span data-ttu-id="0191f-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0191f-124">Property</span></span>|<span data-ttu-id="0191f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0191f-125">Type</span></span>|<span data-ttu-id="0191f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0191f-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0191f-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0191f-127">createdDateTime</span></span>|<span data-ttu-id="0191f-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0191f-128">DateTimeOffset</span></span>|<span data-ttu-id="0191f-129">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="0191f-129">Date and time of creation</span></span>|
|<span data-ttu-id="0191f-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0191f-130">lastSyncDateTime</span></span>|<span data-ttu-id="0191f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0191f-131">DateTimeOffset</span></span>|<span data-ttu-id="0191f-132">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0191f-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="0191f-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0191f-133">applicationVersion</span></span>|<span data-ttu-id="0191f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-134">String</span></span>|<span data-ttu-id="0191f-135">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0191f-135">App version</span></span>|
|<span data-ttu-id="0191f-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0191f-136">managementSdkVersion</span></span>|<span data-ttu-id="0191f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-137">String</span></span>|<span data-ttu-id="0191f-138">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0191f-138">App management SDK version</span></span>|
|<span data-ttu-id="0191f-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="0191f-139">platformVersion</span></span>|<span data-ttu-id="0191f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-140">String</span></span>|<span data-ttu-id="0191f-141">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="0191f-141">Operating System version</span></span>|
|<span data-ttu-id="0191f-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="0191f-142">deviceType</span></span>|<span data-ttu-id="0191f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-143">String</span></span>|<span data-ttu-id="0191f-144">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="0191f-144">Host device type</span></span>|
|<span data-ttu-id="0191f-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0191f-145">deviceTag</span></span>|<span data-ttu-id="0191f-146">String</span><span class="sxs-lookup"><span data-stu-id="0191f-146">String</span></span>|<span data-ttu-id="0191f-147">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0191f-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="0191f-148">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="0191f-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="0191f-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="0191f-149">deviceName</span></span>|<span data-ttu-id="0191f-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-150">String</span></span>|<span data-ttu-id="0191f-151">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="0191f-151">Host device name</span></span>|
|<span data-ttu-id="0191f-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0191f-152">managedDeviceId</span></span>|<span data-ttu-id="0191f-153">String</span><span class="sxs-lookup"><span data-stu-id="0191f-153">String</span></span>|<span data-ttu-id="0191f-154">O identificador de Dispositivo Gerenciado do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="0191f-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="0191f-155">O valor pode estar vazio mesmo quando o dispositivo host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0191f-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="0191f-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0191f-156">azureADDeviceId</span></span>|<span data-ttu-id="0191f-157">String</span><span class="sxs-lookup"><span data-stu-id="0191f-157">String</span></span>|<span data-ttu-id="0191f-158">O identificador do Dispositivo do Azure Active Directory do dispositivo host.</span><span class="sxs-lookup"><span data-stu-id="0191f-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="0191f-159">O valor pode estar vazio mesmo quando o dispositivo host é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0191f-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0191f-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0191f-160">deviceModel</span></span>|<span data-ttu-id="0191f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-161">String</span></span>|<span data-ttu-id="0191f-162">O modelo de dispositivo para o registro de aplicativo atual</span><span class="sxs-lookup"><span data-stu-id="0191f-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="0191f-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="0191f-163">deviceManufacturer</span></span>|<span data-ttu-id="0191f-164">String</span><span class="sxs-lookup"><span data-stu-id="0191f-164">String</span></span>|<span data-ttu-id="0191f-165">O fabricante do dispositivo para o registro atual do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0191f-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="0191f-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="0191f-166">flaggedReasons</span></span>|<span data-ttu-id="0191f-167">[Coleção managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="0191f-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="0191f-168">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0191f-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="0191f-169">E.g.</span><span class="sxs-lookup"><span data-stu-id="0191f-169">E.g.</span></span> <span data-ttu-id="0191f-170">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="0191f-170">app running on rooted device</span></span>|
|<span data-ttu-id="0191f-171">userId</span><span class="sxs-lookup"><span data-stu-id="0191f-171">userId</span></span>|<span data-ttu-id="0191f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0191f-172">String</span></span>|<span data-ttu-id="0191f-173">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="0191f-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="0191f-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0191f-174">appIdentifier</span></span>|[<span data-ttu-id="0191f-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0191f-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="0191f-176">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0191f-176">The app package Identifier</span></span>|
|<span data-ttu-id="0191f-177">id</span><span class="sxs-lookup"><span data-stu-id="0191f-177">id</span></span>|<span data-ttu-id="0191f-178">String</span><span class="sxs-lookup"><span data-stu-id="0191f-178">String</span></span>|<span data-ttu-id="0191f-179">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0191f-179">Key of the entity.</span></span>|
|<span data-ttu-id="0191f-180">versão</span><span class="sxs-lookup"><span data-stu-id="0191f-180">version</span></span>|<span data-ttu-id="0191f-181">String</span><span class="sxs-lookup"><span data-stu-id="0191f-181">String</span></span>|<span data-ttu-id="0191f-182">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0191f-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0191f-183">Relações</span><span class="sxs-lookup"><span data-stu-id="0191f-183">Relationships</span></span>
|<span data-ttu-id="0191f-184">Relação</span><span class="sxs-lookup"><span data-stu-id="0191f-184">Relationship</span></span>|<span data-ttu-id="0191f-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="0191f-185">Type</span></span>|<span data-ttu-id="0191f-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="0191f-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0191f-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="0191f-187">appliedPolicies</span></span>|<span data-ttu-id="0191f-188">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0191f-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0191f-189">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0191f-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="0191f-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="0191f-190">intendedPolicies</span></span>|<span data-ttu-id="0191f-191">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0191f-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0191f-192">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="0191f-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="0191f-193">operations</span><span class="sxs-lookup"><span data-stu-id="0191f-193">operations</span></span>|<span data-ttu-id="0191f-194">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0191f-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="0191f-195">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0191f-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0191f-196">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0191f-196">JSON Representation</span></span>
<span data-ttu-id="0191f-197">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0191f-197">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




