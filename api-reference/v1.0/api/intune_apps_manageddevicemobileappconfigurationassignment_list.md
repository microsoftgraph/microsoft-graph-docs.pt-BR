# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="29aad-101">Listar managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="29aad-101">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="29aad-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="29aad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29aad-103">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="29aad-103">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29aad-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29aad-104">Prerequisites</span></span>
<span data-ttu-id="29aad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29aad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29aad-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29aad-107">Permission type</span></span>|<span data-ttu-id="29aad-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29aad-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29aad-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29aad-109">Delegated (work or school account)</span></span>|<span data-ttu-id="29aad-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29aad-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="29aad-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29aad-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29aad-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29aad-112">Not supported.</span></span>|
|<span data-ttu-id="29aad-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29aad-113">Application</span></span>|<span data-ttu-id="29aad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29aad-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29aad-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29aad-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="29aad-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29aad-116">Request headers</span></span>
|<span data-ttu-id="29aad-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29aad-117">Header</span></span>|<span data-ttu-id="29aad-118">Valor</span><span class="sxs-lookup"><span data-stu-id="29aad-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29aad-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="29aad-119">Authorization</span></span>|<span data-ttu-id="29aad-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29aad-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29aad-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29aad-121">Accept</span></span>|<span data-ttu-id="29aad-122">application/json</span><span class="sxs-lookup"><span data-stu-id="29aad-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29aad-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29aad-123">Request body</span></span>
<span data-ttu-id="29aad-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29aad-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29aad-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="29aad-125">Response</span></span>
<span data-ttu-id="29aad-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29aad-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29aad-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29aad-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="29aad-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29aad-128">Request</span></span>
<span data-ttu-id="29aad-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29aad-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="29aad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="29aad-130">Response</span></span>
<span data-ttu-id="29aad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29aad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



