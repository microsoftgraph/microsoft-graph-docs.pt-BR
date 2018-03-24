# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="2a044-101">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="2a044-101">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="2a044-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a044-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a044-103">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a044-103">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a044-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a044-104">Prerequisites</span></span>
<span data-ttu-id="2a044-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a044-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a044-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a044-107">Permission type</span></span>|<span data-ttu-id="2a044-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a044-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a044-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a044-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a044-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a044-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2a044-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a044-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a044-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a044-112">Not supported.</span></span>|
|<span data-ttu-id="2a044-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a044-113">Application</span></span>|<span data-ttu-id="2a044-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a044-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a044-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a044-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2a044-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a044-116">Request headers</span></span>
|<span data-ttu-id="2a044-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a044-117">Header</span></span>|<span data-ttu-id="2a044-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2a044-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a044-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a044-119">Authorization</span></span>|<span data-ttu-id="2a044-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a044-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a044-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a044-121">Accept</span></span>|<span data-ttu-id="2a044-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a044-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a044-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a044-123">Request body</span></span>
<span data-ttu-id="2a044-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a044-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a044-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a044-125">Response</span></span>
<span data-ttu-id="2a044-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a044-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_onboarding_deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a044-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a044-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a044-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a044-128">Request</span></span>
<span data-ttu-id="2a044-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a044-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="2a044-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a044-130">Response</span></span>
<span data-ttu-id="2a044-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a044-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



