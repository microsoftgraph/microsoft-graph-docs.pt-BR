# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="96ca9-101">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96ca9-101">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="96ca9-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96ca9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96ca9-103">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96ca9-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96ca9-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96ca9-104">Prerequisites</span></span>
<span data-ttu-id="96ca9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96ca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96ca9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96ca9-107">Permission type</span></span>|<span data-ttu-id="96ca9-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96ca9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96ca9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96ca9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96ca9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ca9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96ca9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96ca9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96ca9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96ca9-112">Not supported.</span></span>|
|<span data-ttu-id="96ca9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96ca9-113">Application</span></span>|<span data-ttu-id="96ca9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96ca9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96ca9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96ca9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="96ca9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96ca9-116">Request headers</span></span>
|<span data-ttu-id="96ca9-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96ca9-117">Header</span></span>|<span data-ttu-id="96ca9-118">Valor</span><span class="sxs-lookup"><span data-stu-id="96ca9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96ca9-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="96ca9-119">Authorization</span></span>|<span data-ttu-id="96ca9-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96ca9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96ca9-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96ca9-121">Accept</span></span>|<span data-ttu-id="96ca9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96ca9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ca9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96ca9-123">Request body</span></span>
<span data-ttu-id="96ca9-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96ca9-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="96ca9-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96ca9-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="96ca9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96ca9-126">Property</span></span>|<span data-ttu-id="96ca9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="96ca9-127">Type</span></span>|<span data-ttu-id="96ca9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="96ca9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ca9-129">id</span><span class="sxs-lookup"><span data-stu-id="96ca9-129">id</span></span>|<span data-ttu-id="96ca9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96ca9-130">String</span></span>|<span data-ttu-id="96ca9-131">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="96ca9-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="96ca9-132">target</span><span class="sxs-lookup"><span data-stu-id="96ca9-132">target</span></span>|[<span data-ttu-id="96ca9-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="96ca9-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="96ca9-134">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="96ca9-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="96ca9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96ca9-135">Response</span></span>
<span data-ttu-id="96ca9-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96ca9-136">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ca9-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96ca9-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="96ca9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96ca9-138">Request</span></span>
<span data-ttu-id="96ca9-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96ca9-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="96ca9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="96ca9-140">Response</span></span>
<span data-ttu-id="96ca9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96ca9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



