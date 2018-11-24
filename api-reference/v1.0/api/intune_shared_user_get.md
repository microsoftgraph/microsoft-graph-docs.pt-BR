# <a name="get-user"></a><span data-ttu-id="fa830-101">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="fa830-101">Get user</span></span>

> <span data-ttu-id="fa830-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fa830-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa830-103">Leia as propriedades e as relações do objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="fa830-103">Read properties and relationships of the [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa830-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa830-104">Prerequisites</span></span>
<span data-ttu-id="fa830-105">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fa830-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fa830-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa830-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="fa830-107">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="fa830-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="fa830-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa830-108">Permission type</span></span>|<span data-ttu-id="fa830-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa830-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa830-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa830-110">Delegated (work or school account)</span></span>| <span data-ttu-id="fa830-111">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="fa830-111">_varies by context_</span></span>|
| <span data-ttu-id="fa830-112">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="fa830-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="fa830-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa830-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="fa830-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="fa830-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="fa830-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa830-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="fa830-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="fa830-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="fa830-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa830-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="fa830-118">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="fa830-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="fa830-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa830-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="fa830-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa830-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa830-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa830-121">Not supported.</span></span>|
|<span data-ttu-id="fa830-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa830-122">Application</span></span>|<span data-ttu-id="fa830-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa830-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa830-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa830-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa830-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa830-125">Optional query parameters</span></span>
<span data-ttu-id="fa830-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa830-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fa830-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa830-127">Request headers</span></span>
|<span data-ttu-id="fa830-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa830-128">Header</span></span>|<span data-ttu-id="fa830-129">Valor</span><span class="sxs-lookup"><span data-stu-id="fa830-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa830-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa830-130">Authorization</span></span>|<span data-ttu-id="fa830-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa830-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa830-132">Accept</span><span class="sxs-lookup"><span data-stu-id="fa830-132">Accept</span></span>|<span data-ttu-id="fa830-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fa830-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa830-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa830-134">Request body</span></span>
<span data-ttu-id="fa830-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa830-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa830-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa830-136">Response</span></span>
<span data-ttu-id="fa830-137">Se tiver êxito, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune_shared_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa830-137">If successful, this method returns a `200 OK` response code and [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa830-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa830-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa830-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa830-139">Request</span></span>
<span data-ttu-id="fa830-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa830-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="fa830-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa830-141">Response</span></span>
<span data-ttu-id="fa830-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa830-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



