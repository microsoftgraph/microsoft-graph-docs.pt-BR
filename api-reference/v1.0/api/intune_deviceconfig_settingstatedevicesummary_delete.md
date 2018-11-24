# <a name="delete-settingstatedevicesummary"></a><span data-ttu-id="ea760-101">Excluir settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ea760-101">Delete settingStateDeviceSummary</span></span>

> <span data-ttu-id="ea760-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea760-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea760-103">Exclui [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ea760-103">Deletes a [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea760-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea760-104">Prerequisites</span></span>
<span data-ttu-id="ea760-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea760-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea760-107">Permission type</span></span>|<span data-ttu-id="ea760-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea760-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea760-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea760-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ea760-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea760-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea760-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea760-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea760-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea760-112">Not supported.</span></span>|
|<span data-ttu-id="ea760-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea760-113">Application</span></span>|<span data-ttu-id="ea760-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea760-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea760-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea760-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="ea760-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea760-116">Request headers</span></span>
|<span data-ttu-id="ea760-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea760-117">Header</span></span>|<span data-ttu-id="ea760-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ea760-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea760-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea760-119">Authorization</span></span>|<span data-ttu-id="ea760-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea760-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea760-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea760-121">Accept</span></span>|<span data-ttu-id="ea760-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea760-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea760-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea760-123">Request body</span></span>
<span data-ttu-id="ea760-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea760-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea760-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea760-125">Response</span></span>
<span data-ttu-id="ea760-126">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea760-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea760-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea760-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea760-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea760-128">Request</span></span>
<span data-ttu-id="ea760-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea760-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="ea760-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea760-130">Response</span></span>
<span data-ttu-id="ea760-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea760-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



