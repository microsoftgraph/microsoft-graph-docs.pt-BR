# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="25c7d-101">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="25c7d-101">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="25c7d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="25c7d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25c7d-103">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="25c7d-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25c7d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25c7d-104">Prerequisites</span></span>
<span data-ttu-id="25c7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25c7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25c7d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25c7d-107">Permission type</span></span>|<span data-ttu-id="25c7d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25c7d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c7d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25c7d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="25c7d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c7d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25c7d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25c7d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c7d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25c7d-112">Not supported.</span></span>|
|<span data-ttu-id="25c7d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25c7d-113">Application</span></span>|<span data-ttu-id="25c7d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25c7d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c7d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25c7d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="25c7d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25c7d-116">Request headers</span></span>
|<span data-ttu-id="25c7d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25c7d-117">Header</span></span>|<span data-ttu-id="25c7d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="25c7d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c7d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="25c7d-119">Authorization</span></span>|<span data-ttu-id="25c7d-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="25c7d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c7d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25c7d-121">Accept</span></span>|<span data-ttu-id="25c7d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="25c7d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c7d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25c7d-123">Request body</span></span>
<span data-ttu-id="25c7d-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="25c7d-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="25c7d-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="25c7d-125">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="25c7d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25c7d-126">Property</span></span>|<span data-ttu-id="25c7d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="25c7d-127">Type</span></span>|<span data-ttu-id="25c7d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="25c7d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c7d-129">id</span><span class="sxs-lookup"><span data-stu-id="25c7d-129">id</span></span>|<span data-ttu-id="25c7d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25c7d-130">String</span></span>|<span data-ttu-id="25c7d-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25c7d-131">Key of the entity.</span></span>|
|<span data-ttu-id="25c7d-132">destino</span><span class="sxs-lookup"><span data-stu-id="25c7d-132">target</span></span>|[<span data-ttu-id="25c7d-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="25c7d-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="25c7d-134">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="25c7d-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="25c7d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="25c7d-135">Response</span></span>
<span data-ttu-id="25c7d-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25c7d-136">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c7d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25c7d-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="25c7d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25c7d-138">Request</span></span>
<span data-ttu-id="25c7d-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25c7d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="25c7d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="25c7d-140">Response</span></span>
<span data-ttu-id="25c7d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25c7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








