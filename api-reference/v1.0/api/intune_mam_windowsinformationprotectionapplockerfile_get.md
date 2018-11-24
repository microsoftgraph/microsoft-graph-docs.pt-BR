# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="1ff9a-101">Obter windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="1ff9a-101">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="1ff9a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ff9a-103">Ler propriedades e relações do objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="1ff9a-103">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ff9a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ff9a-104">Prerequisites</span></span>
<span data-ttu-id="1ff9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ff9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ff9a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ff9a-107">Permission type</span></span>|<span data-ttu-id="1ff9a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ff9a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff9a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ff9a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff9a-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff9a-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1ff9a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ff9a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff9a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-112">Not supported.</span></span>|
|<span data-ttu-id="1ff9a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ff9a-113">Application</span></span>|<span data-ttu-id="1ff9a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff9a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff9a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff9a-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ff9a-116">Optional query parameters</span></span>
<span data-ttu-id="1ff9a-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1ff9a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff9a-118">Request headers</span></span>
|<span data-ttu-id="1ff9a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ff9a-119">Header</span></span>|<span data-ttu-id="1ff9a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1ff9a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ff9a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ff9a-121">Authorization</span></span>|<span data-ttu-id="1ff9a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ff9a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ff9a-123">Accept</span></span>|<span data-ttu-id="1ff9a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff9a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff9a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff9a-125">Request body</span></span>
<span data-ttu-id="1ff9a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff9a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff9a-127">Response</span></span>
<span data-ttu-id="1ff9a-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-128">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff9a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ff9a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ff9a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff9a-130">Request</span></span>
<span data-ttu-id="1ff9a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="1ff9a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff9a-132">Response</span></span>
<span data-ttu-id="1ff9a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ff9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```



