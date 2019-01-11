---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7543f7cf591e1e89c05359634b7c4ec55a327b33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825764"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="5ef73-103">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5ef73-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="5ef73-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5ef73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ef73-105">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="5ef73-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="5ef73-106">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="5ef73-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="5ef73-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ef73-107">Methods</span></span>
|<span data-ttu-id="5ef73-108">Método</span><span class="sxs-lookup"><span data-stu-id="5ef73-108">Method</span></span>|<span data-ttu-id="5ef73-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ef73-109">Return Type</span></span>|<span data-ttu-id="5ef73-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef73-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ef73-111">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="5ef73-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="5ef73-112">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef73-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="5ef73-113">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="5ef73-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="5ef73-114">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="5ef73-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="5ef73-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5ef73-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="5ef73-116">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="5ef73-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="5ef73-117">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="5ef73-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="5ef73-118">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5ef73-118">String collection</span></span>|<span data-ttu-id="5ef73-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5ef73-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5ef73-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ef73-120">Properties</span></span>
|<span data-ttu-id="5ef73-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ef73-121">Property</span></span>|<span data-ttu-id="5ef73-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef73-122">Type</span></span>|<span data-ttu-id="5ef73-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef73-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef73-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ef73-124">createdDateTime</span></span>|<span data-ttu-id="5ef73-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ef73-125">DateTimeOffset</span></span>|<span data-ttu-id="5ef73-126">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="5ef73-126">Date and time of creation</span></span>|
|<span data-ttu-id="5ef73-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5ef73-127">lastSyncDateTime</span></span>|<span data-ttu-id="5ef73-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ef73-128">DateTimeOffset</span></span>|<span data-ttu-id="5ef73-129">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5ef73-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="5ef73-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="5ef73-130">applicationVersion</span></span>|<span data-ttu-id="5ef73-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-131">String</span></span>|<span data-ttu-id="5ef73-132">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ef73-132">App version</span></span>|
|<span data-ttu-id="5ef73-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="5ef73-133">managementSdkVersion</span></span>|<span data-ttu-id="5ef73-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-134">String</span></span>|<span data-ttu-id="5ef73-135">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ef73-135">App management SDK version</span></span>|
|<span data-ttu-id="5ef73-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="5ef73-136">platformVersion</span></span>|<span data-ttu-id="5ef73-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-137">String</span></span>|<span data-ttu-id="5ef73-138">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5ef73-138">Operating System version</span></span>|
|<span data-ttu-id="5ef73-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="5ef73-139">deviceType</span></span>|<span data-ttu-id="5ef73-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-140">String</span></span>|<span data-ttu-id="5ef73-141">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="5ef73-141">Host device type</span></span>|
|<span data-ttu-id="5ef73-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="5ef73-142">deviceTag</span></span>|<span data-ttu-id="5ef73-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-143">String</span></span>|<span data-ttu-id="5ef73-144">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ef73-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="5ef73-145">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="5ef73-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="5ef73-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="5ef73-146">deviceName</span></span>|<span data-ttu-id="5ef73-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-147">String</span></span>|<span data-ttu-id="5ef73-148">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="5ef73-148">Host device name</span></span>|
|<span data-ttu-id="5ef73-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="5ef73-149">flaggedReasons</span></span>|<span data-ttu-id="5ef73-150">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="5ef73-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="5ef73-151">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ef73-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="5ef73-152">E.g.</span><span class="sxs-lookup"><span data-stu-id="5ef73-152">E.g.</span></span> <span data-ttu-id="5ef73-153">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="5ef73-153">app running on rooted device</span></span>|
|<span data-ttu-id="5ef73-154">userId</span><span class="sxs-lookup"><span data-stu-id="5ef73-154">userId</span></span>|<span data-ttu-id="5ef73-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-155">String</span></span>|<span data-ttu-id="5ef73-156">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="5ef73-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="5ef73-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ef73-157">appIdentifier</span></span>|[<span data-ttu-id="5ef73-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ef73-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5ef73-159">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ef73-159">The app package Identifier</span></span>|
|<span data-ttu-id="5ef73-160">id</span><span class="sxs-lookup"><span data-stu-id="5ef73-160">id</span></span>|<span data-ttu-id="5ef73-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-161">String</span></span>|<span data-ttu-id="5ef73-162">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ef73-162">Key of the entity.</span></span>|
|<span data-ttu-id="5ef73-163">version</span><span class="sxs-lookup"><span data-stu-id="5ef73-163">version</span></span>|<span data-ttu-id="5ef73-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef73-164">String</span></span>|<span data-ttu-id="5ef73-165">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ef73-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ef73-166">Relações</span><span class="sxs-lookup"><span data-stu-id="5ef73-166">Relationships</span></span>
|<span data-ttu-id="5ef73-167">Relação</span><span class="sxs-lookup"><span data-stu-id="5ef73-167">Relationship</span></span>|<span data-ttu-id="5ef73-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef73-168">Type</span></span>|<span data-ttu-id="5ef73-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef73-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef73-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="5ef73-170">appliedPolicies</span></span>|<span data-ttu-id="5ef73-171">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ef73-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5ef73-172">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5ef73-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="5ef73-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="5ef73-173">intendedPolicies</span></span>|<span data-ttu-id="5ef73-174">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ef73-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5ef73-175">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="5ef73-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="5ef73-176">operations</span><span class="sxs-lookup"><span data-stu-id="5ef73-176">operations</span></span>|<span data-ttu-id="5ef73-177">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="5ef73-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="5ef73-178">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ef73-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ef73-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ef73-179">JSON Representation</span></span>
<span data-ttu-id="5ef73-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ef73-180">Here is a JSON representation of the resource.</span></span>
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
