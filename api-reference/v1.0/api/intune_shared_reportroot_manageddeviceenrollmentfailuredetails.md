# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="e8fd4-101">managedDeviceEnrollmentFailureDetails function</span><span class="sxs-lookup"><span data-stu-id="e8fd4-101">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="e8fd4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8fd4-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8fd4-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8fd4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8fd4-104">Prerequisites</span></span>
<span data-ttu-id="e8fd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8fd4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8fd4-107">Permission type</span></span>|<span data-ttu-id="e8fd4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8fd4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8fd4-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8fd4-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8fd4-110">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e8fd4-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="e8fd4-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fd4-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8fd4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8fd4-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8fd4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-113">Not supported.</span></span>|
|<span data-ttu-id="e8fd4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8fd4-114">Application</span></span>|<span data-ttu-id="e8fd4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8fd4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8fd4-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="e8fd4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fd4-117">Request headers</span></span>
|<span data-ttu-id="e8fd4-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8fd4-118">Header</span></span>|<span data-ttu-id="e8fd4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e8fd4-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8fd4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8fd4-120">Authorization</span></span>|<span data-ttu-id="e8fd4-121">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e8fd4-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8fd4-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8fd4-122">Accept</span></span>|<span data-ttu-id="e8fd4-123">application/json</span><span class="sxs-lookup"><span data-stu-id="e8fd4-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8fd4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fd4-124">Request body</span></span>
<span data-ttu-id="e8fd4-125">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e8fd4-126">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e8fd4-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8fd4-127">Property</span></span>|<span data-ttu-id="e8fd4-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8fd4-128">Type</span></span>|<span data-ttu-id="e8fd4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8fd4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8fd4-130">ignorar</span><span class="sxs-lookup"><span data-stu-id="e8fd4-130">skip</span></span>|<span data-ttu-id="e8fd4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e8fd4-131">Int32</span></span>|<span data-ttu-id="e8fd4-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8fd4-132">Not yet documented</span></span>|
|<span data-ttu-id="e8fd4-133">superior</span><span class="sxs-lookup"><span data-stu-id="e8fd4-133">top</span></span>|<span data-ttu-id="e8fd4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e8fd4-134">Int32</span></span>|<span data-ttu-id="e8fd4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8fd4-135">Not yet documented</span></span>|
|<span data-ttu-id="e8fd4-136">filtro</span><span class="sxs-lookup"><span data-stu-id="e8fd4-136">filter</span></span>|<span data-ttu-id="e8fd4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8fd4-137">String</span></span>|<span data-ttu-id="e8fd4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8fd4-138">Not yet documented</span></span>|
|<span data-ttu-id="e8fd4-139">skipToken</span><span class="sxs-lookup"><span data-stu-id="e8fd4-139">skipToken</span></span>|<span data-ttu-id="e8fd4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8fd4-140">String</span></span>|<span data-ttu-id="e8fd4-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8fd4-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8fd4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8fd4-142">Response</span></span>
<span data-ttu-id="e8fd4-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune_shared_report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-143">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8fd4-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8fd4-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8fd4-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fd4-145">Request</span></span>
<span data-ttu-id="e8fd4-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-146">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e8fd4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8fd4-147">Response</span></span>
<span data-ttu-id="e8fd4-148">O objeto resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-148">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e8fd4-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8fd4-149">All of the properties will be returned from an actual call.</span></span>

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




