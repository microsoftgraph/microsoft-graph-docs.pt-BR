---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 959bd294ab1752617cea6a6ea5bbe8f0a3802f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869717"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="b732a-103">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b732a-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="b732a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b732a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b732a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b732a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b732a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b732a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b732a-107">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b732a-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="b732a-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="b732a-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="b732a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b732a-109">Methods</span></span>
|<span data-ttu-id="b732a-110">Método</span><span class="sxs-lookup"><span data-stu-id="b732a-110">Method</span></span>|<span data-ttu-id="b732a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b732a-111">Return Type</span></span>|<span data-ttu-id="b732a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b732a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b732a-113">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="b732a-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="b732a-114">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="b732a-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="b732a-115">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b732a-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="b732a-116">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="b732a-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="b732a-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b732a-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="b732a-118">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b732a-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="b732a-119">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b732a-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="b732a-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b732a-120">String collection</span></span>|<span data-ttu-id="b732a-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b732a-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b732a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b732a-122">Properties</span></span>
|<span data-ttu-id="b732a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b732a-123">Property</span></span>|<span data-ttu-id="b732a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b732a-124">Type</span></span>|<span data-ttu-id="b732a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b732a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b732a-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b732a-126">createdDateTime</span></span>|<span data-ttu-id="b732a-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b732a-127">DateTimeOffset</span></span>|<span data-ttu-id="b732a-128">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="b732a-128">Date and time of creation</span></span>|
|<span data-ttu-id="b732a-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b732a-129">lastSyncDateTime</span></span>|<span data-ttu-id="b732a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b732a-130">DateTimeOffset</span></span>|<span data-ttu-id="b732a-131">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b732a-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="b732a-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="b732a-132">applicationVersion</span></span>|<span data-ttu-id="b732a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-133">String</span></span>|<span data-ttu-id="b732a-134">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b732a-134">App version</span></span>|
|<span data-ttu-id="b732a-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="b732a-135">managementSdkVersion</span></span>|<span data-ttu-id="b732a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-136">String</span></span>|<span data-ttu-id="b732a-137">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b732a-137">App management SDK version</span></span>|
|<span data-ttu-id="b732a-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="b732a-138">platformVersion</span></span>|<span data-ttu-id="b732a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-139">String</span></span>|<span data-ttu-id="b732a-140">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="b732a-140">Operating System version</span></span>|
|<span data-ttu-id="b732a-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="b732a-141">deviceType</span></span>|<span data-ttu-id="b732a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-142">String</span></span>|<span data-ttu-id="b732a-143">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="b732a-143">Host device type</span></span>|
|<span data-ttu-id="b732a-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b732a-144">deviceTag</span></span>|<span data-ttu-id="b732a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-145">String</span></span>|<span data-ttu-id="b732a-146">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b732a-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="b732a-147">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="b732a-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="b732a-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="b732a-148">deviceName</span></span>|<span data-ttu-id="b732a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-149">String</span></span>|<span data-ttu-id="b732a-150">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="b732a-150">Host device name</span></span>|
|<span data-ttu-id="b732a-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b732a-151">managedDeviceId</span></span>|<span data-ttu-id="b732a-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-152">String</span></span>|<span data-ttu-id="b732a-153">O identificador de dispositivo gerenciado do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="b732a-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="b732a-154">Valor poderia ser vazia, mesmo quando o dispositivo do host é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b732a-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="b732a-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="b732a-155">azureADDeviceId</span></span>|<span data-ttu-id="b732a-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-156">String</span></span>|<span data-ttu-id="b732a-157">O identificador de dispositivo do Azure Active Directory do dispositivo de host.</span><span class="sxs-lookup"><span data-stu-id="b732a-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="b732a-158">Valor poderia ser vazia, mesmo quando o dispositivo do host é o Azure Active Directory registrada.</span><span class="sxs-lookup"><span data-stu-id="b732a-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="b732a-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b732a-159">deviceModel</span></span>|<span data-ttu-id="b732a-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-160">String</span></span>|<span data-ttu-id="b732a-161">O modelo de dispositivo para que o registro atual do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b732a-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="b732a-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="b732a-162">deviceManufacturer</span></span>|<span data-ttu-id="b732a-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-163">String</span></span>|<span data-ttu-id="b732a-164">O fabricante do dispositivo para que o registro atual do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b732a-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="b732a-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="b732a-165">flaggedReasons</span></span>|<span data-ttu-id="b732a-166">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="b732a-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="b732a-167">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b732a-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="b732a-168">E.g.</span><span class="sxs-lookup"><span data-stu-id="b732a-168">E.g.</span></span> <span data-ttu-id="b732a-169">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="b732a-169">app running on rooted device</span></span>|
|<span data-ttu-id="b732a-170">userId</span><span class="sxs-lookup"><span data-stu-id="b732a-170">userId</span></span>|<span data-ttu-id="b732a-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-171">String</span></span>|<span data-ttu-id="b732a-172">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="b732a-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="b732a-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="b732a-173">appIdentifier</span></span>|[<span data-ttu-id="b732a-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b732a-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b732a-175">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b732a-175">The app package Identifier</span></span>|
|<span data-ttu-id="b732a-176">id</span><span class="sxs-lookup"><span data-stu-id="b732a-176">id</span></span>|<span data-ttu-id="b732a-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-177">String</span></span>|<span data-ttu-id="b732a-178">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b732a-178">Key of the entity.</span></span>|
|<span data-ttu-id="b732a-179">version</span><span class="sxs-lookup"><span data-stu-id="b732a-179">version</span></span>|<span data-ttu-id="b732a-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b732a-180">String</span></span>|<span data-ttu-id="b732a-181">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b732a-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b732a-182">Relações</span><span class="sxs-lookup"><span data-stu-id="b732a-182">Relationships</span></span>
|<span data-ttu-id="b732a-183">Relação</span><span class="sxs-lookup"><span data-stu-id="b732a-183">Relationship</span></span>|<span data-ttu-id="b732a-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="b732a-184">Type</span></span>|<span data-ttu-id="b732a-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="b732a-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b732a-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="b732a-186">appliedPolicies</span></span>|<span data-ttu-id="b732a-187">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b732a-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="b732a-188">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b732a-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="b732a-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="b732a-189">intendedPolicies</span></span>|<span data-ttu-id="b732a-190">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b732a-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="b732a-191">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="b732a-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="b732a-192">operations</span><span class="sxs-lookup"><span data-stu-id="b732a-192">operations</span></span>|<span data-ttu-id="b732a-193">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="b732a-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="b732a-194">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b732a-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b732a-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b732a-195">JSON Representation</span></span>
<span data-ttu-id="b732a-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b732a-196">Here is a JSON representation of the resource.</span></span>
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





