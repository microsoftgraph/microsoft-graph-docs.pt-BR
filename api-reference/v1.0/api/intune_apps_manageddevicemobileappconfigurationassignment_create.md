# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="4c7ac-101">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4c7ac-101">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="4c7ac-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c7ac-103">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c7ac-103">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c7ac-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c7ac-104">Prerequisites</span></span>
<span data-ttu-id="4c7ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c7ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c7ac-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c7ac-107">Permission type</span></span>|<span data-ttu-id="4c7ac-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c7ac-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c7ac-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c7ac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c7ac-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7ac-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c7ac-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c7ac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c7ac-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-112">Not supported.</span></span>|
|<span data-ttu-id="4c7ac-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c7ac-113">Application</span></span>|<span data-ttu-id="4c7ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c7ac-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c7ac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4c7ac-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7ac-116">Request headers</span></span>
|<span data-ttu-id="4c7ac-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c7ac-117">Header</span></span>|<span data-ttu-id="4c7ac-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4c7ac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c7ac-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c7ac-119">Authorization</span></span>|<span data-ttu-id="4c7ac-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="4c7ac-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c7ac-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c7ac-121">Accept</span></span>|<span data-ttu-id="4c7ac-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4c7ac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c7ac-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7ac-123">Request body</span></span>
<span data-ttu-id="4c7ac-124">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="4c7ac-125">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="4c7ac-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c7ac-126">Property</span></span>|<span data-ttu-id="4c7ac-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c7ac-127">Type</span></span>|<span data-ttu-id="4c7ac-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c7ac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c7ac-129">id</span><span class="sxs-lookup"><span data-stu-id="4c7ac-129">id</span></span>|<span data-ttu-id="4c7ac-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c7ac-130">String</span></span>|<span data-ttu-id="4c7ac-131">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4c7ac-132">destino</span><span class="sxs-lookup"><span data-stu-id="4c7ac-132">target</span></span>|[<span data-ttu-id="4c7ac-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4c7ac-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4c7ac-134">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="4c7ac-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7ac-135">Response</span></span>
<span data-ttu-id="4c7ac-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-136">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c7ac-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c7ac-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c7ac-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7ac-138">Request</span></span>
<span data-ttu-id="4c7ac-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4c7ac-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7ac-140">Response</span></span>
<span data-ttu-id="4c7ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c7ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








