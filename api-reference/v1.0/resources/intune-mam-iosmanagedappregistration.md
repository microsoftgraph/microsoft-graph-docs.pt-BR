---
title: iosManagedAppRegistration resource type
description: Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0896e848cc83bb2671b0a8d4160ec9dace5ca7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088500"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="75e38-104">iosManagedAppRegistration resource type</span><span class="sxs-lookup"><span data-stu-id="75e38-104">iosManagedAppRegistration resource type</span></span>

<span data-ttu-id="75e38-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75e38-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75e38-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75e38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75e38-107">Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="75e38-107">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="75e38-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="75e38-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="75e38-109">Herda de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75e38-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="75e38-110">Methods</span></span>
|<span data-ttu-id="75e38-111">Método</span><span class="sxs-lookup"><span data-stu-id="75e38-111">Method</span></span>|<span data-ttu-id="75e38-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75e38-112">Return Type</span></span>|<span data-ttu-id="75e38-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="75e38-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75e38-114">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="75e38-114">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="75e38-115">Coleção [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="75e38-116">Lista propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="75e38-116">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="75e38-117">Obter iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="75e38-117">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="75e38-118">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="75e38-118">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="75e38-119">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="75e38-119">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75e38-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75e38-120">Properties</span></span>
|<span data-ttu-id="75e38-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75e38-121">Property</span></span>|<span data-ttu-id="75e38-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="75e38-122">Type</span></span>|<span data-ttu-id="75e38-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="75e38-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75e38-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75e38-124">createdDateTime</span></span>|<span data-ttu-id="75e38-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75e38-125">DateTimeOffset</span></span>|<span data-ttu-id="75e38-126">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-126">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="75e38-127">lastSyncDateTime</span></span>|<span data-ttu-id="75e38-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75e38-128">DateTimeOffset</span></span>|<span data-ttu-id="75e38-129">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="75e38-129">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="75e38-130">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-130">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="75e38-131">applicationVersion</span></span>|<span data-ttu-id="75e38-132">String</span><span class="sxs-lookup"><span data-stu-id="75e38-132">String</span></span>|<span data-ttu-id="75e38-133">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-133">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="75e38-134">managementSdkVersion</span></span>|<span data-ttu-id="75e38-135">String</span><span class="sxs-lookup"><span data-stu-id="75e38-135">String</span></span>|<span data-ttu-id="75e38-136">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-136">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="75e38-137">platformVersion</span></span>|<span data-ttu-id="75e38-138">String</span><span class="sxs-lookup"><span data-stu-id="75e38-138">String</span></span>|<span data-ttu-id="75e38-139">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-139">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="75e38-140">deviceType</span></span>|<span data-ttu-id="75e38-141">String</span><span class="sxs-lookup"><span data-stu-id="75e38-141">String</span></span>|<span data-ttu-id="75e38-142">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-142">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="75e38-143">deviceTag</span></span>|<span data-ttu-id="75e38-144">String</span><span class="sxs-lookup"><span data-stu-id="75e38-144">String</span></span>|<span data-ttu-id="75e38-145">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75e38-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="75e38-146">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="75e38-146">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="75e38-147">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-147">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="75e38-148">deviceName</span></span>|<span data-ttu-id="75e38-149">String</span><span class="sxs-lookup"><span data-stu-id="75e38-149">String</span></span>|<span data-ttu-id="75e38-150">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-150">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="75e38-151">flaggedReasons</span></span>|<span data-ttu-id="75e38-152">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="75e38-153">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75e38-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="75e38-154">E.g.</span><span class="sxs-lookup"><span data-stu-id="75e38-154">E.g.</span></span> <span data-ttu-id="75e38-155">Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-155">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-156">userId</span><span class="sxs-lookup"><span data-stu-id="75e38-156">userId</span></span>|<span data-ttu-id="75e38-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75e38-157">String</span></span>|<span data-ttu-id="75e38-158">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="75e38-158">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="75e38-159">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-159">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-160">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="75e38-160">appIdentifier</span></span>|[<span data-ttu-id="75e38-161">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="75e38-161">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="75e38-162">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-162">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-163">id</span><span class="sxs-lookup"><span data-stu-id="75e38-163">id</span></span>|<span data-ttu-id="75e38-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75e38-164">String</span></span>|<span data-ttu-id="75e38-165">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75e38-165">Key of the entity.</span></span> <span data-ttu-id="75e38-166">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-166">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-167">version</span><span class="sxs-lookup"><span data-stu-id="75e38-167">version</span></span>|<span data-ttu-id="75e38-168">String</span><span class="sxs-lookup"><span data-stu-id="75e38-168">String</span></span>|<span data-ttu-id="75e38-169">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="75e38-169">Version of the entity.</span></span> <span data-ttu-id="75e38-170">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-170">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="75e38-171">Relações</span><span class="sxs-lookup"><span data-stu-id="75e38-171">Relationships</span></span>
|<span data-ttu-id="75e38-172">Relação</span><span class="sxs-lookup"><span data-stu-id="75e38-172">Relationship</span></span>|<span data-ttu-id="75e38-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="75e38-173">Type</span></span>|<span data-ttu-id="75e38-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="75e38-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75e38-175">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="75e38-175">appliedPolicies</span></span>|<span data-ttu-id="75e38-176">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="75e38-177">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="75e38-177">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="75e38-178">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-179">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="75e38-179">intendedPolicies</span></span>|<span data-ttu-id="75e38-180">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="75e38-181">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="75e38-181">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="75e38-182">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-182">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="75e38-183">operations</span><span class="sxs-lookup"><span data-stu-id="75e38-183">operations</span></span>|<span data-ttu-id="75e38-184">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="75e38-185">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75e38-185">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="75e38-186">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="75e38-186">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75e38-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75e38-187">JSON Representation</span></span>
<span data-ttu-id="75e38-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75e38-188">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->







