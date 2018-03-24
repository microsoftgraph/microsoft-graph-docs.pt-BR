# <a name="create-targetedmanagedapppolicyassignment"></a><span data-ttu-id="50dda-101">Criar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="50dda-101">Create targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="50dda-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="50dda-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50dda-103">Criar um novo objeto [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="50dda-103">Create a new [plannerBucket](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50dda-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50dda-104">Prerequisites</span></span>
<span data-ttu-id="50dda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="50dda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50dda-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50dda-107">Permission type</span></span>|<span data-ttu-id="50dda-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50dda-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50dda-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50dda-109">Delegated (work or school account)</span></span>|<span data-ttu-id="50dda-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50dda-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50dda-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50dda-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50dda-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50dda-112">Not supported.</span></span>|
|<span data-ttu-id="50dda-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50dda-113">Application</span></span>|<span data-ttu-id="50dda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50dda-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50dda-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50dda-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="50dda-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50dda-116">Request headers</span></span>
|<span data-ttu-id="50dda-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50dda-117">Header</span></span>|<span data-ttu-id="50dda-118">Valor</span><span class="sxs-lookup"><span data-stu-id="50dda-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50dda-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="50dda-119">Authorization</span></span>|<span data-ttu-id="50dda-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50dda-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="50dda-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50dda-121">Accept</span></span>|<span data-ttu-id="50dda-122">application/json</span><span class="sxs-lookup"><span data-stu-id="50dda-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50dda-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50dda-123">Request body</span></span>
<span data-ttu-id="50dda-124">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="50dda-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="50dda-125">A tabela a seguir mostra as propriedades que são necessárias ao criar targetedManagedAppPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="50dda-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="50dda-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50dda-126">Property</span></span>|<span data-ttu-id="50dda-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="50dda-127">Type</span></span>|<span data-ttu-id="50dda-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="50dda-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50dda-129">id</span><span class="sxs-lookup"><span data-stu-id="50dda-129">id</span></span>|<span data-ttu-id="50dda-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50dda-130">String</span></span>|<span data-ttu-id="50dda-131">Id</span><span class="sxs-lookup"><span data-stu-id="50dda-131">Id</span></span>|
|<span data-ttu-id="50dda-132">target</span><span class="sxs-lookup"><span data-stu-id="50dda-132">target</span></span>|[<span data-ttu-id="50dda-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="50dda-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="50dda-134">Identificador de implantação de um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="50dda-134">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="50dda-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50dda-135">Response</span></span>
<span data-ttu-id="50dda-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50dda-136">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50dda-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50dda-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="50dda-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50dda-138">Request</span></span>
<span data-ttu-id="50dda-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50dda-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="50dda-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50dda-140">Response</span></span>
<span data-ttu-id="50dda-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50dda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



