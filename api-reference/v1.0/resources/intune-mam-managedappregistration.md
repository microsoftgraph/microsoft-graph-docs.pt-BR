---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f825eb1c432490f0fa638e7f753d7db052adee5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066422"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="6cc51-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6cc51-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="6cc51-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cc51-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cc51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cc51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc51-107">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6cc51-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="6cc51-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="6cc51-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="6cc51-109">Methods</span><span class="sxs-lookup"><span data-stu-id="6cc51-109">Methods</span></span>
|<span data-ttu-id="6cc51-110">Método</span><span class="sxs-lookup"><span data-stu-id="6cc51-110">Method</span></span>|<span data-ttu-id="6cc51-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6cc51-111">Return Type</span></span>|<span data-ttu-id="6cc51-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc51-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6cc51-113">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6cc51-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="6cc51-114">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="6cc51-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="6cc51-115">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6cc51-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="6cc51-116">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="6cc51-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="6cc51-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6cc51-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="6cc51-118">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6cc51-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="6cc51-119">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6cc51-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="6cc51-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6cc51-120">String collection</span></span>|<span data-ttu-id="6cc51-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6cc51-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6cc51-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cc51-122">Properties</span></span>
|<span data-ttu-id="6cc51-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cc51-123">Property</span></span>|<span data-ttu-id="6cc51-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cc51-124">Type</span></span>|<span data-ttu-id="6cc51-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc51-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc51-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc51-126">createdDateTime</span></span>|<span data-ttu-id="6cc51-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc51-127">DateTimeOffset</span></span>|<span data-ttu-id="6cc51-128">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="6cc51-128">Date and time of creation</span></span>|
|<span data-ttu-id="6cc51-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc51-129">lastSyncDateTime</span></span>|<span data-ttu-id="6cc51-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc51-130">DateTimeOffset</span></span>|<span data-ttu-id="6cc51-131">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6cc51-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="6cc51-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6cc51-132">applicationVersion</span></span>|<span data-ttu-id="6cc51-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-133">String</span></span>|<span data-ttu-id="6cc51-134">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc51-134">App version</span></span>|
|<span data-ttu-id="6cc51-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6cc51-135">managementSdkVersion</span></span>|<span data-ttu-id="6cc51-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-136">String</span></span>|<span data-ttu-id="6cc51-137">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc51-137">App management SDK version</span></span>|
|<span data-ttu-id="6cc51-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6cc51-138">platformVersion</span></span>|<span data-ttu-id="6cc51-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-139">String</span></span>|<span data-ttu-id="6cc51-140">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="6cc51-140">Operating System version</span></span>|
|<span data-ttu-id="6cc51-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="6cc51-141">deviceType</span></span>|<span data-ttu-id="6cc51-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-142">String</span></span>|<span data-ttu-id="6cc51-143">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="6cc51-143">Host device type</span></span>|
|<span data-ttu-id="6cc51-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6cc51-144">deviceTag</span></span>|<span data-ttu-id="6cc51-145">String</span><span class="sxs-lookup"><span data-stu-id="6cc51-145">String</span></span>|<span data-ttu-id="6cc51-146">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6cc51-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6cc51-147">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="6cc51-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="6cc51-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="6cc51-148">deviceName</span></span>|<span data-ttu-id="6cc51-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-149">String</span></span>|<span data-ttu-id="6cc51-150">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="6cc51-150">Host device name</span></span>|
|<span data-ttu-id="6cc51-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6cc51-151">flaggedReasons</span></span>|<span data-ttu-id="6cc51-152">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="6cc51-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6cc51-153">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cc51-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6cc51-154">E.g.</span><span class="sxs-lookup"><span data-stu-id="6cc51-154">E.g.</span></span> <span data-ttu-id="6cc51-155">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="6cc51-155">app running on rooted device</span></span>|
|<span data-ttu-id="6cc51-156">userId</span><span class="sxs-lookup"><span data-stu-id="6cc51-156">userId</span></span>|<span data-ttu-id="6cc51-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cc51-157">String</span></span>|<span data-ttu-id="6cc51-158">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="6cc51-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="6cc51-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cc51-159">appIdentifier</span></span>|[<span data-ttu-id="6cc51-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cc51-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6cc51-161">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc51-161">The app package Identifier</span></span>|
|<span data-ttu-id="6cc51-162">id</span><span class="sxs-lookup"><span data-stu-id="6cc51-162">id</span></span>|<span data-ttu-id="6cc51-163">String</span><span class="sxs-lookup"><span data-stu-id="6cc51-163">String</span></span>|<span data-ttu-id="6cc51-164">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cc51-164">Key of the entity.</span></span>|
|<span data-ttu-id="6cc51-165">versão</span><span class="sxs-lookup"><span data-stu-id="6cc51-165">version</span></span>|<span data-ttu-id="6cc51-166">String</span><span class="sxs-lookup"><span data-stu-id="6cc51-166">String</span></span>|<span data-ttu-id="6cc51-167">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cc51-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cc51-168">Relações</span><span class="sxs-lookup"><span data-stu-id="6cc51-168">Relationships</span></span>
|<span data-ttu-id="6cc51-169">Relação</span><span class="sxs-lookup"><span data-stu-id="6cc51-169">Relationship</span></span>|<span data-ttu-id="6cc51-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cc51-170">Type</span></span>|<span data-ttu-id="6cc51-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc51-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc51-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="6cc51-172">appliedPolicies</span></span>|<span data-ttu-id="6cc51-173">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6cc51-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6cc51-174">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6cc51-174">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="6cc51-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="6cc51-175">intendedPolicies</span></span>|<span data-ttu-id="6cc51-176">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6cc51-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6cc51-177">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="6cc51-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="6cc51-178">operations</span><span class="sxs-lookup"><span data-stu-id="6cc51-178">operations</span></span>|<span data-ttu-id="6cc51-179">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6cc51-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="6cc51-180">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cc51-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cc51-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cc51-181">JSON Representation</span></span>
<span data-ttu-id="6cc51-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6cc51-182">Here is a JSON representation of the resource.</span></span>
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








