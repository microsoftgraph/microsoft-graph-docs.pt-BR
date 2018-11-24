# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="ad693-101">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ad693-101">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="ad693-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad693-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad693-103">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ad693-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad693-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad693-104">Prerequisites</span></span>
<span data-ttu-id="ad693-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad693-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad693-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad693-107">Permission type</span></span>|<span data-ttu-id="ad693-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad693-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad693-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad693-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad693-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad693-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad693-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad693-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad693-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad693-112">Not supported.</span></span>|
|<span data-ttu-id="ad693-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad693-113">Application</span></span>|<span data-ttu-id="ad693-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad693-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad693-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad693-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ad693-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad693-116">Request headers</span></span>
|<span data-ttu-id="ad693-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad693-117">Header</span></span>|<span data-ttu-id="ad693-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ad693-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad693-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad693-119">Authorization</span></span>|<span data-ttu-id="ad693-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad693-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad693-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad693-121">Accept</span></span>|<span data-ttu-id="ad693-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad693-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad693-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad693-123">Request body</span></span>
<span data-ttu-id="ad693-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="ad693-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="ad693-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="ad693-125">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="ad693-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad693-126">Property</span></span>|<span data-ttu-id="ad693-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad693-127">Type</span></span>|<span data-ttu-id="ad693-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad693-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad693-129">id</span><span class="sxs-lookup"><span data-stu-id="ad693-129">id</span></span>|<span data-ttu-id="ad693-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad693-130">String</span></span>|<span data-ttu-id="ad693-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad693-131">Key of the entity.</span></span>|
|<span data-ttu-id="ad693-132">target</span><span class="sxs-lookup"><span data-stu-id="ad693-132">target</span></span>|[<span data-ttu-id="ad693-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad693-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ad693-134">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ad693-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ad693-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad693-135">Response</span></span>
<span data-ttu-id="ad693-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad693-136">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad693-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad693-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad693-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad693-138">Request</span></span>
<span data-ttu-id="ad693-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad693-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad693-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad693-140">Response</span></span>
<span data-ttu-id="ad693-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad693-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



