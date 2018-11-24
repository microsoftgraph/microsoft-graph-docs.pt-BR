# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="ec9bf-101">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="ec9bf-101">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="ec9bf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec9bf-103">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ec9bf-103">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec9bf-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec9bf-104">Prerequisites</span></span>
<span data-ttu-id="ec9bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec9bf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec9bf-107">Permission type</span></span>|<span data-ttu-id="ec9bf-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec9bf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec9bf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec9bf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec9bf-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec9bf-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ec9bf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec9bf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec9bf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-112">Not supported.</span></span>|
|<span data-ttu-id="ec9bf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec9bf-113">Application</span></span>|<span data-ttu-id="ec9bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec9bf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec9bf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ec9bf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec9bf-116">Request headers</span></span>
|<span data-ttu-id="ec9bf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec9bf-117">Header</span></span>|<span data-ttu-id="ec9bf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ec9bf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec9bf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec9bf-119">Authorization</span></span>|<span data-ttu-id="ec9bf-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec9bf-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec9bf-121">Accept</span></span>|<span data-ttu-id="ec9bf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ec9bf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec9bf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec9bf-123">Request body</span></span>
<span data-ttu-id="ec9bf-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec9bf-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec9bf-125">Response</span></span>
<span data-ttu-id="ec9bf-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-126">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec9bf-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec9bf-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec9bf-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec9bf-128">Request</span></span>
<span data-ttu-id="ec9bf-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="ec9bf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec9bf-130">Response</span></span>
<span data-ttu-id="ec9bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec9bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "members": [
        "Members value"
      ]
    }
  ]
}
```



