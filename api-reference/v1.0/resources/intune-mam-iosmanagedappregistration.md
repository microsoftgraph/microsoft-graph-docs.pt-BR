---
title: iosManagedAppRegistration resource type
description: Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico. O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3971bfb45b4bbdccc64b4d343eb8dea79c055981
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038161"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="79f7d-104">iosManagedAppRegistration resource type</span><span class="sxs-lookup"><span data-stu-id="79f7d-104">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="79f7d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79f7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79f7d-106">Representa os detalhes de sincronização de um aplicativo para iOS, com recursos de gerenciamento, para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="79f7d-106">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="79f7d-107">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="79f7d-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="79f7d-108">Herda de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="79f7d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="79f7d-109">Methods</span></span>
|<span data-ttu-id="79f7d-110">Método</span><span class="sxs-lookup"><span data-stu-id="79f7d-110">Method</span></span>|<span data-ttu-id="79f7d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79f7d-111">Return Type</span></span>|<span data-ttu-id="79f7d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f7d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="79f7d-113">Listar iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="79f7d-113">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="79f7d-114">Coleção [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="79f7d-115">Lista propriedades e relações dos objetos [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="79f7d-115">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="79f7d-116">Obter iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="79f7d-116">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="79f7d-117">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="79f7d-117">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="79f7d-118">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="79f7d-118">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79f7d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79f7d-119">Properties</span></span>
|<span data-ttu-id="79f7d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79f7d-120">Property</span></span>|<span data-ttu-id="79f7d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f7d-121">Type</span></span>|<span data-ttu-id="79f7d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f7d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f7d-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79f7d-123">createdDateTime</span></span>|<span data-ttu-id="79f7d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f7d-124">DateTimeOffset</span></span>|<span data-ttu-id="79f7d-125">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-125">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-126">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="79f7d-126">lastSyncDateTime</span></span>|<span data-ttu-id="79f7d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f7d-127">DateTimeOffset</span></span>|<span data-ttu-id="79f7d-128">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="79f7d-128">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="79f7d-129">Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-129">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="79f7d-130">applicationVersion</span></span>|<span data-ttu-id="79f7d-131">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-131">String</span></span>|<span data-ttu-id="79f7d-132">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-132">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="79f7d-133">managementSdkVersion</span></span>|<span data-ttu-id="79f7d-134">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-134">String</span></span>|<span data-ttu-id="79f7d-135">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-135">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="79f7d-136">platformVersion</span></span>|<span data-ttu-id="79f7d-137">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-137">String</span></span>|<span data-ttu-id="79f7d-138">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-138">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="79f7d-139">deviceType</span></span>|<span data-ttu-id="79f7d-140">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-140">String</span></span>|<span data-ttu-id="79f7d-141">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-141">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="79f7d-142">deviceTag</span></span>|<span data-ttu-id="79f7d-143">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-143">String</span></span>|<span data-ttu-id="79f7d-144">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79f7d-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="79f7d-145">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="79f7d-145">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="79f7d-146">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-146">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="79f7d-147">deviceName</span></span>|<span data-ttu-id="79f7d-148">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-148">String</span></span>|<span data-ttu-id="79f7d-149">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-149">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="79f7d-150">flaggedReasons</span></span>|<span data-ttu-id="79f7d-151">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="79f7d-152">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="79f7d-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="79f7d-153">E.g.</span><span class="sxs-lookup"><span data-stu-id="79f7d-153">E.g.</span></span> <span data-ttu-id="79f7d-154">Aplicativo em execução em um dispositivo root. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-154">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-155">userId</span><span class="sxs-lookup"><span data-stu-id="79f7d-155">userId</span></span>|<span data-ttu-id="79f7d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79f7d-156">String</span></span>|<span data-ttu-id="79f7d-157">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="79f7d-157">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="79f7d-158">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-158">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="79f7d-159">appIdentifier</span></span>|[<span data-ttu-id="79f7d-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="79f7d-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="79f7d-161">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-161">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-162">id</span><span class="sxs-lookup"><span data-stu-id="79f7d-162">id</span></span>|<span data-ttu-id="79f7d-163">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-163">String</span></span>|<span data-ttu-id="79f7d-164">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="79f7d-164">Key of the entity.</span></span> <span data-ttu-id="79f7d-165">Herdado de [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-165">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-166">version</span><span class="sxs-lookup"><span data-stu-id="79f7d-166">version</span></span>|<span data-ttu-id="79f7d-167">String</span><span class="sxs-lookup"><span data-stu-id="79f7d-167">String</span></span>|<span data-ttu-id="79f7d-168">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="79f7d-168">Version of the entity.</span></span> <span data-ttu-id="79f7d-169">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="79f7d-170">Relações</span><span class="sxs-lookup"><span data-stu-id="79f7d-170">Relationships</span></span>
|<span data-ttu-id="79f7d-171">Relação</span><span class="sxs-lookup"><span data-stu-id="79f7d-171">Relationship</span></span>|<span data-ttu-id="79f7d-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f7d-172">Type</span></span>|<span data-ttu-id="79f7d-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f7d-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f7d-174">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="79f7d-174">appliedPolicies</span></span>|<span data-ttu-id="79f7d-175">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="79f7d-176">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="79f7d-176">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="79f7d-177">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-177">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-178">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="79f7d-178">intendedPolicies</span></span>|<span data-ttu-id="79f7d-179">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="79f7d-180">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="79f7d-180">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="79f7d-181">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-181">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="79f7d-182">operations</span><span class="sxs-lookup"><span data-stu-id="79f7d-182">operations</span></span>|<span data-ttu-id="79f7d-183">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="79f7d-184">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="79f7d-184">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="79f7d-185">Herdada da [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7d-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79f7d-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79f7d-186">JSON Representation</span></span>
<span data-ttu-id="79f7d-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79f7d-187">Here is a JSON representation of the resource.</span></span>
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

