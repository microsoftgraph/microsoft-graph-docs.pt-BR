# <a name="managedappregistration-resource-type"></a><span data-ttu-id="268c8-101">Tipo de recurso managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="268c8-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="268c8-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="268c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="268c8-103">O ManagedAppEntity é o tipo de entidade de base para todos os outros tipos de entidades em um fluxo de trabalho de gerenciamento de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="268c8-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="268c8-104">O recurso ManagedAppRegistration representa os detalhes de um aplicativo, com capacidade de gerenciamento, usado por um membro da organização.</span><span class="sxs-lookup"><span data-stu-id="268c8-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="268c8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="268c8-105">Methods</span></span>
|<span data-ttu-id="268c8-106">Método</span><span class="sxs-lookup"><span data-stu-id="268c8-106">Method</span></span>|<span data-ttu-id="268c8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="268c8-107">Return Type</span></span>|<span data-ttu-id="268c8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="268c8-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="268c8-109">Listar managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="268c8-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="268c8-110">Coleção [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="268c8-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="268c8-111">Listar propriedades e relações dos objetos de [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="268c8-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="268c8-112">Obter managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="268c8-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="268c8-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="268c8-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="268c8-114">Ler propriedades e relações do objeto [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="268c8-114">Read properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="268c8-115">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="268c8-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="268c8-116">Coleção String</span><span class="sxs-lookup"><span data-stu-id="268c8-116">String collection</span></span>|<span data-ttu-id="268c8-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="268c8-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="268c8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="268c8-118">Properties</span></span>
|<span data-ttu-id="268c8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="268c8-119">Property</span></span>|<span data-ttu-id="268c8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="268c8-120">Type</span></span>|<span data-ttu-id="268c8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="268c8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="268c8-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="268c8-122">createdDateTime</span></span>|<span data-ttu-id="268c8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="268c8-123">DateTimeOffset</span></span>|<span data-ttu-id="268c8-124">Data e hora de criação</span><span class="sxs-lookup"><span data-stu-id="268c8-124">Date and time of creation</span></span>|
|<span data-ttu-id="268c8-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="268c8-125">lastSyncDateTime</span></span>|<span data-ttu-id="268c8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="268c8-126">DateTimeOffset</span></span>|<span data-ttu-id="268c8-127">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="268c8-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="268c8-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="268c8-128">applicationVersion</span></span>|<span data-ttu-id="268c8-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-129">String</span></span>|<span data-ttu-id="268c8-130">Versão do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="268c8-130">App version</span></span>|
|<span data-ttu-id="268c8-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="268c8-131">managementSdkVersion</span></span>|<span data-ttu-id="268c8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-132">String</span></span>|<span data-ttu-id="268c8-133">Versão do SDK de gerenciamento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="268c8-133">App management SDK version</span></span>|
|<span data-ttu-id="268c8-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="268c8-134">platformVersion</span></span>|<span data-ttu-id="268c8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-135">String</span></span>|<span data-ttu-id="268c8-136">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="268c8-136">Operating System version</span></span>|
|<span data-ttu-id="268c8-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="268c8-137">deviceType</span></span>|<span data-ttu-id="268c8-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-138">String</span></span>|<span data-ttu-id="268c8-139">Tipo de dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="268c8-139">Host device type</span></span>|
|<span data-ttu-id="268c8-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="268c8-140">deviceTag</span></span>|<span data-ttu-id="268c8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-141">String</span></span>|<span data-ttu-id="268c8-142">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="268c8-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="268c8-143">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="268c8-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="268c8-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="268c8-144">deviceName</span></span>|<span data-ttu-id="268c8-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-145">String</span></span>|<span data-ttu-id="268c8-146">Nome do dispositivo do host</span><span class="sxs-lookup"><span data-stu-id="268c8-146">Host device name</span></span>|
|<span data-ttu-id="268c8-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="268c8-147">flaggedReasons</span></span>|<span data-ttu-id="268c8-148">coleção [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="268c8-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="268c8-149">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="268c8-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="268c8-150">E.g.</span><span class="sxs-lookup"><span data-stu-id="268c8-150">E.g.</span></span> <span data-ttu-id="268c8-151">aplicativo usado em dispositivo modificado</span><span class="sxs-lookup"><span data-stu-id="268c8-151">app running on rooted device</span></span>|
|<span data-ttu-id="268c8-152">userId</span><span class="sxs-lookup"><span data-stu-id="268c8-152">userId</span></span>|<span data-ttu-id="268c8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-153">String</span></span>|<span data-ttu-id="268c8-154">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="268c8-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="268c8-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="268c8-155">appIdentifier</span></span>|[<span data-ttu-id="268c8-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="268c8-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="268c8-157">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="268c8-157">The app package Identifier</span></span>|
|<span data-ttu-id="268c8-158">id</span><span class="sxs-lookup"><span data-stu-id="268c8-158">id</span></span>|<span data-ttu-id="268c8-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-159">String</span></span>|<span data-ttu-id="268c8-160">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="268c8-160">Key of the entity.</span></span>|
|<span data-ttu-id="268c8-161">version</span><span class="sxs-lookup"><span data-stu-id="268c8-161">version</span></span>|<span data-ttu-id="268c8-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="268c8-162">String</span></span>|<span data-ttu-id="268c8-163">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="268c8-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="268c8-164">Relações</span><span class="sxs-lookup"><span data-stu-id="268c8-164">Relationships</span></span>
|<span data-ttu-id="268c8-165">Relação</span><span class="sxs-lookup"><span data-stu-id="268c8-165">Relationship</span></span>|<span data-ttu-id="268c8-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="268c8-166">Type</span></span>|<span data-ttu-id="268c8-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="268c8-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="268c8-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="268c8-168">appliedPolicies</span></span>|<span data-ttu-id="268c8-169">Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="268c8-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="268c8-170">Zero ou mais políticas já aplicadas no aplicativo registrado quando este foi sincronizado pela última vez com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="268c8-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="268c8-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="268c8-171">intendedPolicies</span></span>|<span data-ttu-id="268c8-172">Coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="268c8-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="268c8-173">Zero ou mais administradores de políticas destinados ao aplicativo a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="268c8-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="268c8-174">operations</span><span class="sxs-lookup"><span data-stu-id="268c8-174">operations</span></span>|<span data-ttu-id="268c8-175">Coleção [managedAppOperation](../resources/intune_mam_managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="268c8-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="268c8-176">Zero ou mais operações de longa execução desencadeadas no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="268c8-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="268c8-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="268c8-177">JSON Representation</span></span>
<span data-ttu-id="268c8-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="268c8-178">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
