# <a name="get-devicemanagement"></a><span data-ttu-id="f68d1-101">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f68d1-101">Get deviceManagement</span></span>

> <span data-ttu-id="f68d1-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f68d1-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f68d1-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f68d1-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f68d1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f68d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f68d1-105">Ler propriedades e relações do objeto [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f68d1-105">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f68d1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f68d1-106">Prerequisites</span></span>
<span data-ttu-id="f68d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f68d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f68d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f68d1-109">Permission type</span></span>|<span data-ttu-id="f68d1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f68d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f68d1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f68d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f68d1-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f68d1-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f68d1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f68d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f68d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f68d1-114">Not supported.</span></span>|
|<span data-ttu-id="f68d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f68d1-115">Application</span></span>|<span data-ttu-id="f68d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f68d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f68d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f68d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f68d1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f68d1-118">Optional query parameters</span></span>
<span data-ttu-id="f68d1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f68d1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f68d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f68d1-120">Request headers</span></span>
|<span data-ttu-id="f68d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f68d1-121">Header</span></span>|<span data-ttu-id="f68d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f68d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f68d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f68d1-123">Authorization</span></span>|<span data-ttu-id="f68d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f68d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f68d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f68d1-125">Accept</span></span>|<span data-ttu-id="f68d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f68d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f68d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f68d1-127">Request body</span></span>
<span data-ttu-id="f68d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f68d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f68d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f68d1-129">Response</span></span>
<span data-ttu-id="f68d1-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f68d1-130">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f68d1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f68d1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f68d1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f68d1-132">Request</span></span>
<span data-ttu-id="f68d1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f68d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="f68d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f68d1-134">Response</span></span>
<span data-ttu-id="f68d1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f68d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```



