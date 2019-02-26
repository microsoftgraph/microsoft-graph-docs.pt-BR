---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4754a190f19dab34ac417d2852ccc9e06ba9f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252235"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="8e380-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8e380-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="8e380-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e380-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e380-106">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8e380-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="8e380-107">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="8e380-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8e380-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e380-108">Methods</span></span>
|<span data-ttu-id="8e380-109">Método</span><span class="sxs-lookup"><span data-stu-id="8e380-109">Method</span></span>|<span data-ttu-id="8e380-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e380-110">Return Type</span></span>|<span data-ttu-id="8e380-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e380-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e380-112">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="8e380-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="8e380-113">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8e380-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="8e380-114">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8e380-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="8e380-115">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="8e380-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="8e380-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8e380-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="8e380-117">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8e380-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="8e380-118">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8e380-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="8e380-119">Coleção String</span><span class="sxs-lookup"><span data-stu-id="8e380-119">String collection</span></span>|<span data-ttu-id="8e380-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8e380-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8e380-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e380-121">Properties</span></span>
|<span data-ttu-id="8e380-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e380-122">Property</span></span>|<span data-ttu-id="8e380-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e380-123">Type</span></span>|<span data-ttu-id="8e380-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e380-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e380-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e380-125">createdDateTime</span></span>|<span data-ttu-id="8e380-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e380-126">DateTimeOffset</span></span>|<span data-ttu-id="8e380-127">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="8e380-127">Date and time of creation</span></span>|
|<span data-ttu-id="8e380-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e380-128">lastSyncDateTime</span></span>|<span data-ttu-id="8e380-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e380-129">DateTimeOffset</span></span>|<span data-ttu-id="8e380-130">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="8e380-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="8e380-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8e380-131">applicationVersion</span></span>|<span data-ttu-id="8e380-132">String</span><span class="sxs-lookup"><span data-stu-id="8e380-132">String</span></span>|<span data-ttu-id="8e380-133">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e380-133">App version</span></span>|
|<span data-ttu-id="8e380-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8e380-134">managementSdkVersion</span></span>|<span data-ttu-id="8e380-135">String</span><span class="sxs-lookup"><span data-stu-id="8e380-135">String</span></span>|<span data-ttu-id="8e380-136">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e380-136">App management SDK version</span></span>|
|<span data-ttu-id="8e380-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8e380-137">platformVersion</span></span>|<span data-ttu-id="8e380-138">String</span><span class="sxs-lookup"><span data-stu-id="8e380-138">String</span></span>|<span data-ttu-id="8e380-139">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="8e380-139">Operating System version</span></span>|
|<span data-ttu-id="8e380-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="8e380-140">deviceType</span></span>|<span data-ttu-id="8e380-141">String</span><span class="sxs-lookup"><span data-stu-id="8e380-141">String</span></span>|<span data-ttu-id="8e380-142">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="8e380-142">Host device type</span></span>|
|<span data-ttu-id="8e380-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8e380-143">deviceTag</span></span>|<span data-ttu-id="8e380-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e380-144">String</span></span>|<span data-ttu-id="8e380-145">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e380-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8e380-146">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="8e380-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="8e380-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="8e380-147">deviceName</span></span>|<span data-ttu-id="8e380-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e380-148">String</span></span>|<span data-ttu-id="8e380-149">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="8e380-149">Host device name</span></span>|
|<span data-ttu-id="8e380-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8e380-150">flaggedReasons</span></span>|<span data-ttu-id="8e380-151">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="8e380-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="8e380-152">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e380-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8e380-153">E.g.</span><span class="sxs-lookup"><span data-stu-id="8e380-153">E.g.</span></span> <span data-ttu-id="8e380-154">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="8e380-154">app running on rooted device</span></span>|
|<span data-ttu-id="8e380-155">userId</span><span class="sxs-lookup"><span data-stu-id="8e380-155">userId</span></span>|<span data-ttu-id="8e380-156">String</span><span class="sxs-lookup"><span data-stu-id="8e380-156">String</span></span>|<span data-ttu-id="8e380-157">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="8e380-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="8e380-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e380-158">appIdentifier</span></span>|[<span data-ttu-id="8e380-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e380-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8e380-160">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e380-160">The app package Identifier</span></span>|
|<span data-ttu-id="8e380-161">id</span><span class="sxs-lookup"><span data-stu-id="8e380-161">id</span></span>|<span data-ttu-id="8e380-162">String</span><span class="sxs-lookup"><span data-stu-id="8e380-162">String</span></span>|<span data-ttu-id="8e380-163">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e380-163">Key of the entity.</span></span>|
|<span data-ttu-id="8e380-164">version</span><span class="sxs-lookup"><span data-stu-id="8e380-164">version</span></span>|<span data-ttu-id="8e380-165">String</span><span class="sxs-lookup"><span data-stu-id="8e380-165">String</span></span>|<span data-ttu-id="8e380-166">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e380-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e380-167">Relações</span><span class="sxs-lookup"><span data-stu-id="8e380-167">Relationships</span></span>
|<span data-ttu-id="8e380-168">Relação</span><span class="sxs-lookup"><span data-stu-id="8e380-168">Relationship</span></span>|<span data-ttu-id="8e380-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e380-169">Type</span></span>|<span data-ttu-id="8e380-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e380-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e380-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="8e380-171">appliedPolicies</span></span>|<span data-ttu-id="8e380-172">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e380-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8e380-173">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="8e380-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="8e380-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="8e380-174">intendedPolicies</span></span>|<span data-ttu-id="8e380-175">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e380-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8e380-176">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="8e380-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="8e380-177">operations</span><span class="sxs-lookup"><span data-stu-id="8e380-177">operations</span></span>|<span data-ttu-id="8e380-178">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8e380-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="8e380-179">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e380-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e380-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e380-180">JSON Representation</span></span>
<span data-ttu-id="8e380-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e380-181">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


