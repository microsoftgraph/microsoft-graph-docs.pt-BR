# <a name="delete-devicecompliancescheduledactionforrule"></a><span data-ttu-id="6089c-101">Excluir deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="6089c-101">Delete deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="6089c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6089c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6089c-103">Exclui [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6089c-103">Deletes a [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6089c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6089c-104">Prerequisites</span></span>
<span data-ttu-id="6089c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6089c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6089c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6089c-107">Permission type</span></span>|<span data-ttu-id="6089c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6089c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6089c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6089c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6089c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6089c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6089c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6089c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6089c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6089c-112">Not supported.</span></span>|
|<span data-ttu-id="6089c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6089c-113">Application</span></span>|<span data-ttu-id="6089c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6089c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6089c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6089c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="6089c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6089c-116">Request headers</span></span>
|<span data-ttu-id="6089c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6089c-117">Header</span></span>|<span data-ttu-id="6089c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6089c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6089c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6089c-119">Authorization</span></span>|<span data-ttu-id="6089c-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6089c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6089c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6089c-121">Accept</span></span>|<span data-ttu-id="6089c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6089c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6089c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6089c-123">Request body</span></span>
<span data-ttu-id="6089c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6089c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6089c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6089c-125">Response</span></span>
<span data-ttu-id="6089c-126">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6089c-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6089c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6089c-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="6089c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6089c-128">Request</span></span>
<span data-ttu-id="6089c-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6089c-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="6089c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6089c-130">Response</span></span>
<span data-ttu-id="6089c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6089c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



