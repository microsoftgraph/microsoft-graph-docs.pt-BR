# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="06395-101">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="06395-101">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="06395-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06395-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06395-103">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="06395-103">Create a new [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06395-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06395-104">Prerequisites</span></span>
<span data-ttu-id="06395-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06395-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06395-107">Permission type</span></span>|<span data-ttu-id="06395-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06395-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06395-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06395-109">Delegated (work or school account)</span></span>|<span data-ttu-id="06395-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06395-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06395-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06395-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06395-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06395-112">Not supported.</span></span>|
|<span data-ttu-id="06395-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06395-113">Application</span></span>|<span data-ttu-id="06395-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06395-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06395-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06395-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="06395-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06395-116">Request headers</span></span>
|<span data-ttu-id="06395-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06395-117">Header</span></span>|<span data-ttu-id="06395-118">Valor</span><span class="sxs-lookup"><span data-stu-id="06395-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06395-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="06395-119">Authorization</span></span>|<span data-ttu-id="06395-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="06395-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06395-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06395-121">Accept</span></span>|<span data-ttu-id="06395-122">application/json</span><span class="sxs-lookup"><span data-stu-id="06395-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06395-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06395-123">Request body</span></span>
<span data-ttu-id="06395-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="06395-124">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="06395-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="06395-125">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="06395-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06395-126">Property</span></span>|<span data-ttu-id="06395-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="06395-127">Type</span></span>|<span data-ttu-id="06395-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="06395-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06395-129">id</span><span class="sxs-lookup"><span data-stu-id="06395-129">id</span></span>|<span data-ttu-id="06395-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06395-130">String</span></span>|<span data-ttu-id="06395-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06395-131">Key of the entity.</span></span>|
|<span data-ttu-id="06395-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="06395-132">ruleName</span></span>|<span data-ttu-id="06395-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06395-133">String</span></span>|<span data-ttu-id="06395-134">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="06395-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="06395-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06395-135">Response</span></span>
<span data-ttu-id="06395-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06395-136">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06395-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06395-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="06395-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06395-138">Request</span></span>
<span data-ttu-id="06395-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06395-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="06395-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="06395-140">Response</span></span>
<span data-ttu-id="06395-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06395-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```








