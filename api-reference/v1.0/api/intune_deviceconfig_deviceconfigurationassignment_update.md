# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="dd58f-101">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="dd58f-101">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="dd58f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd58f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd58f-103">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd58f-103">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd58f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd58f-104">Prerequisites</span></span>
<span data-ttu-id="dd58f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd58f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd58f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd58f-107">Permission type</span></span>|<span data-ttu-id="dd58f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd58f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd58f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd58f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dd58f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd58f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd58f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd58f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd58f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd58f-112">Not supported.</span></span>|
|<span data-ttu-id="dd58f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd58f-113">Application</span></span>|<span data-ttu-id="dd58f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd58f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd58f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd58f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="dd58f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd58f-116">Request headers</span></span>
|<span data-ttu-id="dd58f-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd58f-117">Header</span></span>|<span data-ttu-id="dd58f-118">Valor</span><span class="sxs-lookup"><span data-stu-id="dd58f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd58f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd58f-119">Authorization</span></span>|<span data-ttu-id="dd58f-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="dd58f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd58f-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd58f-121">Accept</span></span>|<span data-ttu-id="dd58f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dd58f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd58f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd58f-123">Request body</span></span>
<span data-ttu-id="dd58f-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd58f-124">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="dd58f-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd58f-125">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="dd58f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd58f-126">Property</span></span>|<span data-ttu-id="dd58f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd58f-127">Type</span></span>|<span data-ttu-id="dd58f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd58f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd58f-129">id</span><span class="sxs-lookup"><span data-stu-id="dd58f-129">id</span></span>|<span data-ttu-id="dd58f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd58f-130">String</span></span>|<span data-ttu-id="dd58f-131">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="dd58f-131">The key of the assignment.</span></span>|
|<span data-ttu-id="dd58f-132">destino</span><span class="sxs-lookup"><span data-stu-id="dd58f-132">target</span></span>|[<span data-ttu-id="dd58f-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dd58f-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dd58f-134">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd58f-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="dd58f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd58f-135">Response</span></span>
<span data-ttu-id="dd58f-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd58f-136">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd58f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd58f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd58f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd58f-138">Request</span></span>
<span data-ttu-id="dd58f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd58f-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="dd58f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd58f-140">Response</span></span>
<span data-ttu-id="dd58f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd58f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








