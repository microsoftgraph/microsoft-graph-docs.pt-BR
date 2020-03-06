---
title: iosManagedAppRegistration resource type
description: Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4ff8bbf35b021ca6dac4e9cad1bbda42de61f8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530205"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="d1ccd-104">iosManagedAppRegistration resource type</span><span class="sxs-lookup"><span data-stu-id="d1ccd-104">iosManagedAppRegistration resource type</span></span>

<span data-ttu-id="d1ccd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1ccd-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1ccd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ccd-107">Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-107">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="d1ccd-108">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="d1ccd-109">Herda de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d1ccd-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="d1ccd-110">Methods</span></span>
|<span data-ttu-id="d1ccd-111">Método</span><span class="sxs-lookup"><span data-stu-id="d1ccd-111">Method</span></span>|<span data-ttu-id="d1ccd-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d1ccd-112">Return Type</span></span>|<span data-ttu-id="d1ccd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ccd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1ccd-114">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d1ccd-114">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="d1ccd-115">Coleção [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="d1ccd-116">Lista propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d1ccd-116">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d1ccd-117">Obter iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d1ccd-117">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="d1ccd-118">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d1ccd-118">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="d1ccd-119">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d1ccd-119">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1ccd-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1ccd-120">Properties</span></span>
|<span data-ttu-id="d1ccd-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1ccd-121">Property</span></span>|<span data-ttu-id="d1ccd-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1ccd-122">Type</span></span>|<span data-ttu-id="d1ccd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ccd-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ccd-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1ccd-124">createdDateTime</span></span>|<span data-ttu-id="d1ccd-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1ccd-125">DateTimeOffset</span></span>|<span data-ttu-id="d1ccd-126">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-126">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d1ccd-127">lastSyncDateTime</span></span>|<span data-ttu-id="d1ccd-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1ccd-128">DateTimeOffset</span></span>|<span data-ttu-id="d1ccd-129">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-129">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d1ccd-130">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-130">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d1ccd-131">applicationVersion</span></span>|<span data-ttu-id="d1ccd-132">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-132">String</span></span>|<span data-ttu-id="d1ccd-133">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-133">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d1ccd-134">managementSdkVersion</span></span>|<span data-ttu-id="d1ccd-135">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-135">String</span></span>|<span data-ttu-id="d1ccd-136">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-136">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d1ccd-137">platformVersion</span></span>|<span data-ttu-id="d1ccd-138">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-138">String</span></span>|<span data-ttu-id="d1ccd-139">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-139">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="d1ccd-140">deviceType</span></span>|<span data-ttu-id="d1ccd-141">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-141">String</span></span>|<span data-ttu-id="d1ccd-142">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-142">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d1ccd-143">deviceTag</span></span>|<span data-ttu-id="d1ccd-144">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-144">String</span></span>|<span data-ttu-id="d1ccd-145">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d1ccd-146">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-146">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d1ccd-147">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-147">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="d1ccd-148">deviceName</span></span>|<span data-ttu-id="d1ccd-149">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-149">String</span></span>|<span data-ttu-id="d1ccd-150">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-150">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d1ccd-151">flaggedReasons</span></span>|<span data-ttu-id="d1ccd-152">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d1ccd-153">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d1ccd-154">E.g.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-154">E.g.</span></span> <span data-ttu-id="d1ccd-155">Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-155">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-156">userId</span><span class="sxs-lookup"><span data-stu-id="d1ccd-156">userId</span></span>|<span data-ttu-id="d1ccd-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1ccd-157">String</span></span>|<span data-ttu-id="d1ccd-158">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-158">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d1ccd-159">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-159">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-160">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1ccd-160">appIdentifier</span></span>|[<span data-ttu-id="d1ccd-161">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1ccd-161">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d1ccd-162">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-162">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-163">id</span><span class="sxs-lookup"><span data-stu-id="d1ccd-163">id</span></span>|<span data-ttu-id="d1ccd-164">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-164">String</span></span>|<span data-ttu-id="d1ccd-165">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-165">Key of the entity.</span></span> <span data-ttu-id="d1ccd-166">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-166">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-167">version</span><span class="sxs-lookup"><span data-stu-id="d1ccd-167">version</span></span>|<span data-ttu-id="d1ccd-168">String</span><span class="sxs-lookup"><span data-stu-id="d1ccd-168">String</span></span>|<span data-ttu-id="d1ccd-169">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-169">Version of the entity.</span></span> <span data-ttu-id="d1ccd-170">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-170">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1ccd-171">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d1ccd-171">Relationships</span></span>
|<span data-ttu-id="d1ccd-172">Relação</span><span class="sxs-lookup"><span data-stu-id="d1ccd-172">Relationship</span></span>|<span data-ttu-id="d1ccd-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1ccd-173">Type</span></span>|<span data-ttu-id="d1ccd-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ccd-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ccd-175">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d1ccd-175">appliedPolicies</span></span>|<span data-ttu-id="d1ccd-176">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d1ccd-177">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-177">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="d1ccd-178">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-179">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d1ccd-179">intendedPolicies</span></span>|<span data-ttu-id="d1ccd-180">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d1ccd-181">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-181">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="d1ccd-182">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-182">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d1ccd-183">operations</span><span class="sxs-lookup"><span data-stu-id="d1ccd-183">operations</span></span>|<span data-ttu-id="d1ccd-184">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d1ccd-185">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-185">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="d1ccd-186">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ccd-186">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1ccd-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1ccd-187">JSON Representation</span></span>
<span data-ttu-id="d1ccd-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1ccd-188">Here is a JSON representation of the resource.</span></span>
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


