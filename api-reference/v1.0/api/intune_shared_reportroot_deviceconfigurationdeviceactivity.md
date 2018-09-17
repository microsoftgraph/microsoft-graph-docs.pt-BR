# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="ae9df-101">Função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="ae9df-101">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="ae9df-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ae9df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae9df-103">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ae9df-103">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae9df-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae9df-104">Prerequisites</span></span>
<span data-ttu-id="ae9df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae9df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae9df-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae9df-107">Permission type</span></span>|<span data-ttu-id="ae9df-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae9df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae9df-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae9df-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ae9df-110">&nbsp; &nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ae9df-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="ae9df-111">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae9df-111">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae9df-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae9df-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae9df-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae9df-113">Not supported.</span></span>|
|<span data-ttu-id="ae9df-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae9df-114">Application</span></span>|<span data-ttu-id="ae9df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae9df-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae9df-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae9df-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="ae9df-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae9df-117">Request headers</span></span>
|<span data-ttu-id="ae9df-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae9df-118">Header</span></span>|<span data-ttu-id="ae9df-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ae9df-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae9df-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae9df-120">Authorization</span></span>|<span data-ttu-id="ae9df-121">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ae9df-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae9df-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae9df-122">Accept</span></span>|<span data-ttu-id="ae9df-123">application/json</span><span class="sxs-lookup"><span data-stu-id="ae9df-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae9df-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae9df-124">Request body</span></span>
<span data-ttu-id="ae9df-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae9df-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae9df-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae9df-126">Response</span></span>
<span data-ttu-id="ae9df-127">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune_shared_report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae9df-127">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae9df-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae9df-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae9df-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae9df-129">Request</span></span>
<span data-ttu-id="ae9df-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae9df-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="ae9df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae9df-131">Response</span></span>
<span data-ttu-id="ae9df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae9df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








