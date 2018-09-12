# <a name="get-editionupgradeconfiguration"></a><span data-ttu-id="d666f-101">Obter o editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d666f-101">Get editionUpgradeConfiguration</span></span>

> <span data-ttu-id="d666f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d666f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d666f-103">Ler propriedades e relações do objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d666f-103">Read properties and relationships of the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d666f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d666f-104">Prerequisites</span></span>
<span data-ttu-id="d666f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d666f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d666f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d666f-107">Permission type</span></span>|<span data-ttu-id="d666f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d666f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d666f-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d666f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d666f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d666f-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d666f-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d666f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d666f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d666f-112">Not supported.</span></span>|
|<span data-ttu-id="d666f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d666f-113">Application</span></span>|<span data-ttu-id="d666f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d666f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d666f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d666f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d666f-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d666f-116">Optional query parameters</span></span>
<span data-ttu-id="d666f-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d666f-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d666f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d666f-118">Request headers</span></span>
|<span data-ttu-id="d666f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d666f-119">Header</span></span>|<span data-ttu-id="d666f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d666f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d666f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d666f-121">Authorization</span></span>|<span data-ttu-id="d666f-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d666f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d666f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d666f-123">Accept</span></span>|<span data-ttu-id="d666f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d666f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d666f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d666f-125">Request body</span></span>
<span data-ttu-id="d666f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d666f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d666f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d666f-127">Response</span></span>
<span data-ttu-id="d666f-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d666f-128">If successful, this method returns a `200 OK` response code and [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d666f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d666f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d666f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d666f-130">Request</span></span>
<span data-ttu-id="d666f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d666f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d666f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d666f-132">Response</span></span>
<span data-ttu-id="d666f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d666f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": {
    "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
    "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "licenseType": "licenseFile",
    "targetEdition": "windows10EnterpriseN",
    "license": "License value",
    "productKey": "Product Key value"
  }
}
```








