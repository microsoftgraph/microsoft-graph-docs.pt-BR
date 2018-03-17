# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="a4c31-101">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4c31-101">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a4c31-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a4c31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4c31-103">Ler propriedades e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4c31-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4c31-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4c31-104">Prerequisites</span></span>
<span data-ttu-id="a4c31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4c31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4c31-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c31-107">Permission type</span></span>|<span data-ttu-id="a4c31-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4c31-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4c31-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c31-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a4c31-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4c31-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4c31-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c31-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4c31-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c31-112">Not supported.</span></span>|
|<span data-ttu-id="a4c31-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c31-113">Application</span></span>|<span data-ttu-id="a4c31-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c31-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4c31-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c31-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4c31-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4c31-116">Optional query parameters</span></span>
<span data-ttu-id="a4c31-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c31-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4c31-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c31-118">Request headers</span></span>
|<span data-ttu-id="a4c31-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4c31-119">Header</span></span>|<span data-ttu-id="a4c31-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a4c31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4c31-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4c31-121">Authorization</span></span>|<span data-ttu-id="a4c31-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4c31-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4c31-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4c31-123">Accept</span></span>|<span data-ttu-id="a4c31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4c31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4c31-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c31-125">Request body</span></span>
<span data-ttu-id="a4c31-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4c31-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4c31-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c31-127">Response</span></span>
<span data-ttu-id="a4c31-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c31-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4c31-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4c31-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4c31-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c31-130">Request</span></span>
<span data-ttu-id="a4c31-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4c31-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a4c31-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c31-132">Response</span></span>
<span data-ttu-id="a4c31-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4c31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1155

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumCharacterSetCount": 0,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true
  }
}
```



