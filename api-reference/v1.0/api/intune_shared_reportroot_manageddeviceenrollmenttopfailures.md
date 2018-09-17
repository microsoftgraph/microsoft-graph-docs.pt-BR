# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="be110-101">Função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="be110-101">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="be110-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="be110-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be110-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be110-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be110-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be110-104">Prerequisites</span></span>
<span data-ttu-id="be110-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be110-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be110-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be110-107">Permission type</span></span>|<span data-ttu-id="be110-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be110-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be110-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be110-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be110-110">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="be110-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="be110-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be110-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be110-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be110-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be110-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be110-113">Not supported.</span></span>|
|<span data-ttu-id="be110-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be110-114">Application</span></span>|<span data-ttu-id="be110-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be110-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be110-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be110-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="be110-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be110-117">Request headers</span></span>
|<span data-ttu-id="be110-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be110-118">Header</span></span>|<span data-ttu-id="be110-119">Valor</span><span class="sxs-lookup"><span data-stu-id="be110-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be110-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="be110-120">Authorization</span></span>|<span data-ttu-id="be110-121">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="be110-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be110-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be110-122">Accept</span></span>|<span data-ttu-id="be110-123">application/json</span><span class="sxs-lookup"><span data-stu-id="be110-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be110-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be110-124">Request body</span></span>
<span data-ttu-id="be110-125">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="be110-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="be110-126">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="be110-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="be110-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be110-127">Property</span></span>|<span data-ttu-id="be110-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="be110-128">Type</span></span>|<span data-ttu-id="be110-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="be110-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be110-130">período</span><span class="sxs-lookup"><span data-stu-id="be110-130">period</span></span>|<span data-ttu-id="be110-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be110-131">String</span></span>|<span data-ttu-id="be110-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be110-132">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="be110-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="be110-133">Response</span></span>
<span data-ttu-id="be110-134">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune_shared_report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be110-134">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be110-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be110-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="be110-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be110-136">Request</span></span>
<span data-ttu-id="be110-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be110-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="be110-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="be110-138">Response</span></span>
<span data-ttu-id="be110-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be110-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




