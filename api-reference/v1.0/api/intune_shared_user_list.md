# <a name="list-users"></a><span data-ttu-id="2d235-101">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="2d235-101">List users</span></span>

> <span data-ttu-id="2d235-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d235-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d235-103">Listar propriedades e relações de objetos de [usuário](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="2d235-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d235-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d235-104">Prerequisites</span></span>
<span data-ttu-id="2d235-105">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2d235-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="2d235-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d235-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="2d235-107">A permissão específica requerida depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="2d235-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="2d235-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d235-108">Permission type</span></span>|<span data-ttu-id="2d235-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d235-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d235-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d235-110">Delegated (work or school account)</span></span>| <span data-ttu-id="2d235-111">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="2d235-111">_varies by context_</span></span>|
| <span data-ttu-id="2d235-112">&nbsp; &nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="2d235-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="2d235-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d235-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="2d235-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="2d235-114">.mam</span></span> | <span data-ttu-id="2d235-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d235-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="2d235-116">&nbsp; &nbsp; Nível de contratação</span><span class="sxs-lookup"><span data-stu-id="2d235-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="2d235-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d235-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="2d235-118">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="2d235-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="2d235-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d235-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="2d235-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d235-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d235-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d235-121">Not supported.</span></span>|
|<span data-ttu-id="2d235-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d235-122">Application</span></span>|<span data-ttu-id="2d235-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d235-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d235-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d235-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="2d235-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d235-125">Request headers</span></span>
|<span data-ttu-id="2d235-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d235-126">Header</span></span>|<span data-ttu-id="2d235-127">Valor</span><span class="sxs-lookup"><span data-stu-id="2d235-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d235-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d235-128">Authorization</span></span>|<span data-ttu-id="2d235-129">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="2d235-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d235-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d235-130">Accept</span></span>|<span data-ttu-id="2d235-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2d235-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d235-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d235-132">Request body</span></span>
<span data-ttu-id="2d235-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d235-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d235-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d235-134">Response</span></span>
<span data-ttu-id="2d235-135">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune_shared_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d235-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d235-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d235-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d235-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d235-137">Request</span></span>
<span data-ttu-id="2d235-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d235-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="2d235-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d235-139">Response</span></span>
<span data-ttu-id="2d235-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d235-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



