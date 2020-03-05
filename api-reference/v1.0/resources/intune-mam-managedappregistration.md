---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 964850f0b4a8cbd2ceed152460385eb4fadf037b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448337"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="696f8-104">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="696f8-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="696f8-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="696f8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="696f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="696f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="696f8-107">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="696f8-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="696f8-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="696f8-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="696f8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="696f8-109">Methods</span></span>
|<span data-ttu-id="696f8-110">Método</span><span class="sxs-lookup"><span data-stu-id="696f8-110">Method</span></span>|<span data-ttu-id="696f8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="696f8-111">Return Type</span></span>|<span data-ttu-id="696f8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="696f8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="696f8-113">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="696f8-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="696f8-114">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="696f8-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="696f8-115">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="696f8-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="696f8-116">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="696f8-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="696f8-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="696f8-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="696f8-118">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="696f8-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="696f8-119">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="696f8-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="696f8-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="696f8-120">String collection</span></span>|<span data-ttu-id="696f8-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="696f8-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="696f8-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="696f8-122">Properties</span></span>
|<span data-ttu-id="696f8-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="696f8-123">Property</span></span>|<span data-ttu-id="696f8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="696f8-124">Type</span></span>|<span data-ttu-id="696f8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="696f8-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696f8-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="696f8-126">createdDateTime</span></span>|<span data-ttu-id="696f8-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696f8-127">DateTimeOffset</span></span>|<span data-ttu-id="696f8-128">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="696f8-128">Date and time of creation</span></span>|
|<span data-ttu-id="696f8-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="696f8-129">lastSyncDateTime</span></span>|<span data-ttu-id="696f8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696f8-130">DateTimeOffset</span></span>|<span data-ttu-id="696f8-131">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="696f8-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="696f8-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="696f8-132">applicationVersion</span></span>|<span data-ttu-id="696f8-133">String</span><span class="sxs-lookup"><span data-stu-id="696f8-133">String</span></span>|<span data-ttu-id="696f8-134">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="696f8-134">App version</span></span>|
|<span data-ttu-id="696f8-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="696f8-135">managementSdkVersion</span></span>|<span data-ttu-id="696f8-136">String</span><span class="sxs-lookup"><span data-stu-id="696f8-136">String</span></span>|<span data-ttu-id="696f8-137">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="696f8-137">App management SDK version</span></span>|
|<span data-ttu-id="696f8-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="696f8-138">platformVersion</span></span>|<span data-ttu-id="696f8-139">String</span><span class="sxs-lookup"><span data-stu-id="696f8-139">String</span></span>|<span data-ttu-id="696f8-140">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="696f8-140">Operating System version</span></span>|
|<span data-ttu-id="696f8-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="696f8-141">deviceType</span></span>|<span data-ttu-id="696f8-142">String</span><span class="sxs-lookup"><span data-stu-id="696f8-142">String</span></span>|<span data-ttu-id="696f8-143">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="696f8-143">Host device type</span></span>|
|<span data-ttu-id="696f8-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="696f8-144">deviceTag</span></span>|<span data-ttu-id="696f8-145">String</span><span class="sxs-lookup"><span data-stu-id="696f8-145">String</span></span>|<span data-ttu-id="696f8-146">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="696f8-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="696f8-147">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="696f8-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="696f8-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="696f8-148">deviceName</span></span>|<span data-ttu-id="696f8-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="696f8-149">String</span></span>|<span data-ttu-id="696f8-150">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="696f8-150">Host device name</span></span>|
|<span data-ttu-id="696f8-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="696f8-151">flaggedReasons</span></span>|<span data-ttu-id="696f8-152">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="696f8-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="696f8-153">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="696f8-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="696f8-154">E.g.</span><span class="sxs-lookup"><span data-stu-id="696f8-154">E.g.</span></span> <span data-ttu-id="696f8-155">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="696f8-155">app running on rooted device</span></span>|
|<span data-ttu-id="696f8-156">userId</span><span class="sxs-lookup"><span data-stu-id="696f8-156">userId</span></span>|<span data-ttu-id="696f8-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="696f8-157">String</span></span>|<span data-ttu-id="696f8-158">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="696f8-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="696f8-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="696f8-159">appIdentifier</span></span>|[<span data-ttu-id="696f8-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="696f8-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="696f8-161">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="696f8-161">The app package Identifier</span></span>|
|<span data-ttu-id="696f8-162">id</span><span class="sxs-lookup"><span data-stu-id="696f8-162">id</span></span>|<span data-ttu-id="696f8-163">String</span><span class="sxs-lookup"><span data-stu-id="696f8-163">String</span></span>|<span data-ttu-id="696f8-164">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="696f8-164">Key of the entity.</span></span>|
|<span data-ttu-id="696f8-165">versão</span><span class="sxs-lookup"><span data-stu-id="696f8-165">version</span></span>|<span data-ttu-id="696f8-166">String</span><span class="sxs-lookup"><span data-stu-id="696f8-166">String</span></span>|<span data-ttu-id="696f8-167">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="696f8-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="696f8-168">Relações</span><span class="sxs-lookup"><span data-stu-id="696f8-168">Relationships</span></span>
|<span data-ttu-id="696f8-169">Relação</span><span class="sxs-lookup"><span data-stu-id="696f8-169">Relationship</span></span>|<span data-ttu-id="696f8-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="696f8-170">Type</span></span>|<span data-ttu-id="696f8-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="696f8-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696f8-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="696f8-172">appliedPolicies</span></span>|<span data-ttu-id="696f8-173">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="696f8-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="696f8-174">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="696f8-174">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="696f8-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="696f8-175">intendedPolicies</span></span>|<span data-ttu-id="696f8-176">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="696f8-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="696f8-177">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="696f8-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="696f8-178">operations</span><span class="sxs-lookup"><span data-stu-id="696f8-178">operations</span></span>|<span data-ttu-id="696f8-179">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="696f8-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="696f8-180">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="696f8-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="696f8-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="696f8-181">JSON Representation</span></span>
<span data-ttu-id="696f8-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="696f8-182">Here is a JSON representation of the resource.</span></span>
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



