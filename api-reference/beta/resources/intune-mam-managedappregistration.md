---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421435"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="d15d9-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d15d9-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="d15d9-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d15d9-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d15d9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d15d9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d15d9-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d15d9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d15d9-108">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d15d9-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="d15d9-109">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="d15d9-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="d15d9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="d15d9-110">Methods</span></span>
|<span data-ttu-id="d15d9-111">Método</span><span class="sxs-lookup"><span data-stu-id="d15d9-111">Method</span></span>|<span data-ttu-id="d15d9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d15d9-112">Return Type</span></span>|<span data-ttu-id="d15d9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15d9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d15d9-114">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d15d9-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="d15d9-115">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d15d9-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="d15d9-116">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d15d9-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d15d9-117">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d15d9-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="d15d9-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d15d9-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="d15d9-119">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d15d9-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="d15d9-120">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d15d9-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="d15d9-121">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d15d9-121">String collection</span></span>|<span data-ttu-id="d15d9-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d15d9-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d15d9-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d15d9-123">Properties</span></span>
|<span data-ttu-id="d15d9-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d15d9-124">Property</span></span>|<span data-ttu-id="d15d9-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d15d9-125">Type</span></span>|<span data-ttu-id="d15d9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15d9-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d15d9-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d15d9-127">createdDateTime</span></span>|<span data-ttu-id="d15d9-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d15d9-128">DateTimeOffset</span></span>|<span data-ttu-id="d15d9-129">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="d15d9-129">Date and time of creation</span></span>|
|<span data-ttu-id="d15d9-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d15d9-130">lastSyncDateTime</span></span>|<span data-ttu-id="d15d9-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d15d9-131">DateTimeOffset</span></span>|<span data-ttu-id="d15d9-132">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d15d9-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="d15d9-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d15d9-133">applicationVersion</span></span>|<span data-ttu-id="d15d9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-134">String</span></span>|<span data-ttu-id="d15d9-135">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15d9-135">App version</span></span>|
|<span data-ttu-id="d15d9-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d15d9-136">managementSdkVersion</span></span>|<span data-ttu-id="d15d9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-137">String</span></span>|<span data-ttu-id="d15d9-138">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15d9-138">App management SDK version</span></span>|
|<span data-ttu-id="d15d9-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d15d9-139">platformVersion</span></span>|<span data-ttu-id="d15d9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-140">String</span></span>|<span data-ttu-id="d15d9-141">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d15d9-141">Operating System version</span></span>|
|<span data-ttu-id="d15d9-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="d15d9-142">deviceType</span></span>|<span data-ttu-id="d15d9-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-143">String</span></span>|<span data-ttu-id="d15d9-144">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="d15d9-144">Host device type</span></span>|
|<span data-ttu-id="d15d9-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d15d9-145">deviceTag</span></span>|<span data-ttu-id="d15d9-146">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-146">String</span></span>|<span data-ttu-id="d15d9-147">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d15d9-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d15d9-148">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="d15d9-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="d15d9-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="d15d9-149">deviceName</span></span>|<span data-ttu-id="d15d9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-150">String</span></span>|<span data-ttu-id="d15d9-151">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="d15d9-151">Host device name</span></span>|
|<span data-ttu-id="d15d9-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d15d9-152">managedDeviceId</span></span>|<span data-ttu-id="d15d9-153">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-153">String</span></span>|<span data-ttu-id="d15d9-154">O identificador de dispositivo gerenciado do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="d15d9-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="d15d9-155">Valor poderia ser vazia, mesmo quando o dispositivo do host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d15d9-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="d15d9-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d15d9-156">azureADDeviceId</span></span>|<span data-ttu-id="d15d9-157">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-157">String</span></span>|<span data-ttu-id="d15d9-158">O identificador de dispositivo do Azure Active Directory do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="d15d9-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="d15d9-159">Valor poderia ser vazia, mesmo quando o dispositivo do host é o Azure Active Directory registrada.</span><span class="sxs-lookup"><span data-stu-id="d15d9-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d15d9-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d15d9-160">deviceModel</span></span>|<span data-ttu-id="d15d9-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15d9-161">String</span></span>|<span data-ttu-id="d15d9-162">O modelo de dispositivo para que o registro atual do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15d9-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="d15d9-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="d15d9-163">deviceManufacturer</span></span>|<span data-ttu-id="d15d9-164">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-164">String</span></span>|<span data-ttu-id="d15d9-165">O fabricante do dispositivo para que o registro atual do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15d9-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="d15d9-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d15d9-166">flaggedReasons</span></span>|<span data-ttu-id="d15d9-167">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="d15d9-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d15d9-168">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d15d9-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d15d9-169">E.g.</span><span class="sxs-lookup"><span data-stu-id="d15d9-169">E.g.</span></span> <span data-ttu-id="d15d9-170">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="d15d9-170">app running on rooted device</span></span>|
|<span data-ttu-id="d15d9-171">userId</span><span class="sxs-lookup"><span data-stu-id="d15d9-171">userId</span></span>|<span data-ttu-id="d15d9-172">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-172">String</span></span>|<span data-ttu-id="d15d9-173">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="d15d9-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="d15d9-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d15d9-174">appIdentifier</span></span>|[<span data-ttu-id="d15d9-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d15d9-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d15d9-176">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15d9-176">The app package Identifier</span></span>|
|<span data-ttu-id="d15d9-177">id</span><span class="sxs-lookup"><span data-stu-id="d15d9-177">id</span></span>|<span data-ttu-id="d15d9-178">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-178">String</span></span>|<span data-ttu-id="d15d9-179">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d15d9-179">Key of the entity.</span></span>|
|<span data-ttu-id="d15d9-180">version</span><span class="sxs-lookup"><span data-stu-id="d15d9-180">version</span></span>|<span data-ttu-id="d15d9-181">String</span><span class="sxs-lookup"><span data-stu-id="d15d9-181">String</span></span>|<span data-ttu-id="d15d9-182">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d15d9-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d15d9-183">Relações</span><span class="sxs-lookup"><span data-stu-id="d15d9-183">Relationships</span></span>
|<span data-ttu-id="d15d9-184">Relação</span><span class="sxs-lookup"><span data-stu-id="d15d9-184">Relationship</span></span>|<span data-ttu-id="d15d9-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="d15d9-185">Type</span></span>|<span data-ttu-id="d15d9-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15d9-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d15d9-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d15d9-187">appliedPolicies</span></span>|<span data-ttu-id="d15d9-188">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d15d9-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d15d9-189">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d15d9-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="d15d9-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d15d9-190">intendedPolicies</span></span>|<span data-ttu-id="d15d9-191">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d15d9-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d15d9-192">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="d15d9-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="d15d9-193">operations</span><span class="sxs-lookup"><span data-stu-id="d15d9-193">operations</span></span>|<span data-ttu-id="d15d9-194">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="d15d9-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d15d9-195">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d15d9-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d15d9-196">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d15d9-196">JSON Representation</span></span>
<span data-ttu-id="d15d9-197">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d15d9-197">Here is a JSON representation of the resource.</span></span>
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




