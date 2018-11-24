# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="a2c13-101">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a2c13-101">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="a2c13-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a2c13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2c13-103">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a2c13-103">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2c13-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2c13-104">Prerequisites</span></span>
<span data-ttu-id="a2c13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2c13-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2c13-107">Permission type</span></span>|<span data-ttu-id="a2c13-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2c13-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2c13-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2c13-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2c13-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2c13-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2c13-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2c13-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2c13-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2c13-112">Not supported.</span></span>|
|<span data-ttu-id="a2c13-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2c13-113">Application</span></span>|<span data-ttu-id="a2c13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2c13-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2c13-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2c13-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a2c13-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c13-116">Request headers</span></span>
|<span data-ttu-id="a2c13-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2c13-117">Header</span></span>|<span data-ttu-id="a2c13-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a2c13-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2c13-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2c13-119">Authorization</span></span>|<span data-ttu-id="a2c13-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2c13-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2c13-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2c13-121">Accept</span></span>|<span data-ttu-id="a2c13-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a2c13-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2c13-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c13-123">Request body</span></span>
<span data-ttu-id="a2c13-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2c13-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2c13-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c13-125">Response</span></span>
<span data-ttu-id="a2c13-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2c13-126">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2c13-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2c13-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2c13-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c13-128">Request</span></span>
<span data-ttu-id="a2c13-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2c13-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="a2c13-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c13-130">Response</span></span>
<span data-ttu-id="a2c13-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2c13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



