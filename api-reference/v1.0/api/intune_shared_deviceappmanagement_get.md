# <a name="get-deviceappmanagement"></a><span data-ttu-id="8ef4b-101">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="8ef4b-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="8ef4b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ef4b-103">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8ef4b-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ef4b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ef4b-104">Prerequisites</span></span>

<span data-ttu-id="8ef4b-105">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8ef4b-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ef4b-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="8ef4b-107">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="8ef4b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ef4b-108">Permission type</span></span>|<span data-ttu-id="8ef4b-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ef4b-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ef4b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ef4b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8ef4b-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ef4b-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="8ef4b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ef4b-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ef4b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-113">Not supported.</span></span>|
|<span data-ttu-id="8ef4b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ef4b-114">Application</span></span>|<span data-ttu-id="8ef4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ef4b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ef4b-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ef4b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ef4b-117">Optional query parameters</span></span>
<span data-ttu-id="8ef4b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ef4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ef4b-119">Request headers</span></span>
|<span data-ttu-id="8ef4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ef4b-120">Header</span></span>|<span data-ttu-id="8ef4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8ef4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ef4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ef4b-122">Authorization</span></span>|<span data-ttu-id="8ef4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ef4b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8ef4b-124">Accept</span></span>|<span data-ttu-id="8ef4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ef4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ef4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ef4b-126">Request body</span></span>
<span data-ttu-id="8ef4b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ef4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ef4b-128">Response</span></span>
<span data-ttu-id="8ef4b-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="8ef4b-130">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ef4b-130">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="8ef4b-131">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="8ef4b-131">Example response</span></span>
<span data-ttu-id="8ef4b-132">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8ef4b-133">Serão retornadas todas as propriedades de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-133">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



