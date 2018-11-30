---
title: Tipo de recurso managedAppRegistration
description: O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.
ms.openlocfilehash: efccea80c953ee4eac07588a21944d10810f8532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004180"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="88e30-103">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="88e30-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="88e30-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="88e30-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88e30-105">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="88e30-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="88e30-106">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="88e30-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="88e30-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="88e30-107">Methods</span></span>
|<span data-ttu-id="88e30-108">Método</span><span class="sxs-lookup"><span data-stu-id="88e30-108">Method</span></span>|<span data-ttu-id="88e30-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88e30-109">Return Type</span></span>|<span data-ttu-id="88e30-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88e30-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88e30-111">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="88e30-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="88e30-112">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="88e30-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="88e30-113">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="88e30-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="88e30-114">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="88e30-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="88e30-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="88e30-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="88e30-116">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="88e30-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="88e30-117">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="88e30-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="88e30-118">Coleção String</span><span class="sxs-lookup"><span data-stu-id="88e30-118">String collection</span></span>|<span data-ttu-id="88e30-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="88e30-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="88e30-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88e30-120">Properties</span></span>
|<span data-ttu-id="88e30-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88e30-121">Property</span></span>|<span data-ttu-id="88e30-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="88e30-122">Type</span></span>|<span data-ttu-id="88e30-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="88e30-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88e30-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88e30-124">createdDateTime</span></span>|<span data-ttu-id="88e30-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88e30-125">DateTimeOffset</span></span>|<span data-ttu-id="88e30-126">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="88e30-126">Date and time of creation</span></span>|
|<span data-ttu-id="88e30-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="88e30-127">lastSyncDateTime</span></span>|<span data-ttu-id="88e30-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88e30-128">DateTimeOffset</span></span>|<span data-ttu-id="88e30-129">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="88e30-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="88e30-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="88e30-130">applicationVersion</span></span>|<span data-ttu-id="88e30-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88e30-131">String</span></span>|<span data-ttu-id="88e30-132">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88e30-132">App version</span></span>|
|<span data-ttu-id="88e30-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="88e30-133">managementSdkVersion</span></span>|<span data-ttu-id="88e30-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88e30-134">String</span></span>|<span data-ttu-id="88e30-135">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="88e30-135">App management SDK version</span></span>|
|<span data-ttu-id="88e30-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="88e30-136">platformVersion</span></span>|<span data-ttu-id="88e30-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88e30-137">String</span></span>|<span data-ttu-id="88e30-138">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="88e30-138">Operating System version</span></span>|
|<span data-ttu-id="88e30-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="88e30-139">deviceType</span></span>|<span data-ttu-id="88e30-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88e30-140">String</span></span>|<span data-ttu-id="88e30-141">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="88e30-141">Host device type</span></span>|
|<span data-ttu-id="88e30-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="88e30-142">deviceTag</span></span>|<span data-ttu-id="88e30-143">String</span><span class="sxs-lookup"><span data-stu-id="88e30-143">String</span></span>|<span data-ttu-id="88e30-144">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88e30-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="88e30-145">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="88e30-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="88e30-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="88e30-146">deviceName</span></span>|<span data-ttu-id="88e30-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88e30-147">String</span></span>|<span data-ttu-id="88e30-148">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="88e30-148">Host device name</span></span>|
|<span data-ttu-id="88e30-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="88e30-149">flaggedReasons</span></span>|<span data-ttu-id="88e30-150">coleção [managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="88e30-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="88e30-151">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88e30-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="88e30-152">E.g.</span><span class="sxs-lookup"><span data-stu-id="88e30-152">E.g.</span></span> <span data-ttu-id="88e30-153">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="88e30-153">app running on rooted device</span></span>|
|<span data-ttu-id="88e30-154">userId</span><span class="sxs-lookup"><span data-stu-id="88e30-154">userId</span></span>|<span data-ttu-id="88e30-155">String</span><span class="sxs-lookup"><span data-stu-id="88e30-155">String</span></span>|<span data-ttu-id="88e30-156">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="88e30-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="88e30-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="88e30-157">appIdentifier</span></span>|[<span data-ttu-id="88e30-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="88e30-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="88e30-159">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="88e30-159">The app package Identifier</span></span>|
|<span data-ttu-id="88e30-160">id</span><span class="sxs-lookup"><span data-stu-id="88e30-160">id</span></span>|<span data-ttu-id="88e30-161">String</span><span class="sxs-lookup"><span data-stu-id="88e30-161">String</span></span>|<span data-ttu-id="88e30-162">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88e30-162">Key of the entity.</span></span>|
|<span data-ttu-id="88e30-163">version</span><span class="sxs-lookup"><span data-stu-id="88e30-163">version</span></span>|<span data-ttu-id="88e30-164">String</span><span class="sxs-lookup"><span data-stu-id="88e30-164">String</span></span>|<span data-ttu-id="88e30-165">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="88e30-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88e30-166">Relações</span><span class="sxs-lookup"><span data-stu-id="88e30-166">Relationships</span></span>
|<span data-ttu-id="88e30-167">Relação</span><span class="sxs-lookup"><span data-stu-id="88e30-167">Relationship</span></span>|<span data-ttu-id="88e30-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="88e30-168">Type</span></span>|<span data-ttu-id="88e30-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="88e30-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88e30-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="88e30-170">appliedPolicies</span></span>|<span data-ttu-id="88e30-171">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88e30-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="88e30-172">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="88e30-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="88e30-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="88e30-173">intendedPolicies</span></span>|<span data-ttu-id="88e30-174">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88e30-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="88e30-175">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="88e30-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="88e30-176">operations</span><span class="sxs-lookup"><span data-stu-id="88e30-176">operations</span></span>|<span data-ttu-id="88e30-177">Coleção [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="88e30-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="88e30-178">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="88e30-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88e30-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88e30-179">JSON Representation</span></span>
<span data-ttu-id="88e30-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88e30-180">Here is a JSON representation of the resource.</span></span>
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
