# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="6f0cd-101">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6f0cd-101">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="6f0cd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f0cd-103">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f0cd-103">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f0cd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f0cd-104">Prerequisites</span></span>
<span data-ttu-id="6f0cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f0cd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f0cd-107">Permission type</span></span>|<span data-ttu-id="6f0cd-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f0cd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f0cd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f0cd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f0cd-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f0cd-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f0cd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f0cd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f0cd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-112">Not supported.</span></span>|
|<span data-ttu-id="6f0cd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f0cd-113">Application</span></span>|<span data-ttu-id="6f0cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f0cd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f0cd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6f0cd-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0cd-116">Request headers</span></span>
|<span data-ttu-id="6f0cd-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f0cd-117">Header</span></span>|<span data-ttu-id="6f0cd-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6f0cd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f0cd-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f0cd-119">Authorization</span></span>|<span data-ttu-id="6f0cd-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="6f0cd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f0cd-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f0cd-121">Accept</span></span>|<span data-ttu-id="6f0cd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6f0cd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f0cd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0cd-123">Request body</span></span>
<span data-ttu-id="6f0cd-124">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f0cd-124">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6f0cd-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6f0cd-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="6f0cd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f0cd-126">Property</span></span>|<span data-ttu-id="6f0cd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f0cd-127">Type</span></span>|<span data-ttu-id="6f0cd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f0cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f0cd-129">id</span><span class="sxs-lookup"><span data-stu-id="6f0cd-129">id</span></span>|<span data-ttu-id="6f0cd-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f0cd-130">String</span></span>|<span data-ttu-id="6f0cd-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6f0cd-131">Not yet documented</span></span>|
|<span data-ttu-id="6f0cd-132">destino</span><span class="sxs-lookup"><span data-stu-id="6f0cd-132">target</span></span>|[<span data-ttu-id="6f0cd-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6f0cd-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6f0cd-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6f0cd-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f0cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f0cd-135">Response</span></span>
<span data-ttu-id="6f0cd-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-136">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f0cd-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f0cd-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f0cd-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0cd-138">Request</span></span>
<span data-ttu-id="6f0cd-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6f0cd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f0cd-140">Response</span></span>
<span data-ttu-id="6f0cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f0cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



