# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="2a695-101">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2a695-101">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="2a695-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a695-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a695-103">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a695-103">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a695-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a695-104">Prerequisites</span></span>
<span data-ttu-id="2a695-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a695-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a695-107">Permission type</span></span>|<span data-ttu-id="2a695-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a695-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a695-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a695-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a695-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a695-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a695-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a695-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a695-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a695-112">Not supported.</span></span>|
|<span data-ttu-id="2a695-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a695-113">Application</span></span>|<span data-ttu-id="2a695-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a695-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a695-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a695-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2a695-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a695-116">Request headers</span></span>
|<span data-ttu-id="2a695-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a695-117">Header</span></span>|<span data-ttu-id="2a695-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2a695-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a695-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a695-119">Authorization</span></span>|<span data-ttu-id="2a695-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a695-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a695-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a695-121">Accept</span></span>|<span data-ttu-id="2a695-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a695-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a695-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a695-123">Request body</span></span>
<span data-ttu-id="2a695-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a695-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="2a695-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a695-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="2a695-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a695-126">Property</span></span>|<span data-ttu-id="2a695-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a695-127">Type</span></span>|<span data-ttu-id="2a695-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a695-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a695-129">id</span><span class="sxs-lookup"><span data-stu-id="2a695-129">id</span></span>|<span data-ttu-id="2a695-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a695-130">String</span></span>|<span data-ttu-id="2a695-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a695-131">Key of the entity.</span></span>|
|<span data-ttu-id="2a695-132">target</span><span class="sxs-lookup"><span data-stu-id="2a695-132">target</span></span>|[<span data-ttu-id="2a695-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a695-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a695-134">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2a695-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2a695-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a695-135">Response</span></span>
<span data-ttu-id="2a695-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a695-136">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a695-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a695-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a695-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a695-138">Request</span></span>
<span data-ttu-id="2a695-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a695-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2a695-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a695-140">Response</span></span>
<span data-ttu-id="2a695-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a695-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



