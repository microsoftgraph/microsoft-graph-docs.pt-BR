# <a name="update-user"></a><span data-ttu-id="d0a92-101">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="d0a92-101">Update user</span></span>

> <span data-ttu-id="d0a92-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d0a92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0a92-103">Atualizar as propriedades de um objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="d0a92-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0a92-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0a92-104">Prerequisites</span></span>
<span data-ttu-id="d0a92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0a92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0a92-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0a92-107">Permission type</span></span>|<span data-ttu-id="d0a92-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0a92-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0a92-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0a92-109">Delegated (work or school account)</span></span>| <span data-ttu-id="d0a92-110">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="d0a92-110">_varies by context_</span></span>|
| <span data-ttu-id="d0a92-111">&nbsp; &nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="d0a92-111">&nbsp;&nbsp;</span></span> | <span data-ttu-id="d0a92-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a92-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d0a92-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="d0a92-113">.mam</span></span> | <span data-ttu-id="d0a92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a92-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d0a92-115">&nbsp; &nbsp; Nível de contratação</span><span class="sxs-lookup"><span data-stu-id="d0a92-115">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="d0a92-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a92-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d0a92-117">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="d0a92-117">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="d0a92-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a92-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="d0a92-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0a92-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0a92-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0a92-120">Not supported.</span></span>|
|<span data-ttu-id="d0a92-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0a92-121">Application</span></span>|<span data-ttu-id="d0a92-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0a92-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0a92-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0a92-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d0a92-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a92-124">Request headers</span></span>
|<span data-ttu-id="d0a92-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0a92-125">Header</span></span>|<span data-ttu-id="d0a92-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d0a92-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0a92-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0a92-127">Authorization</span></span>|<span data-ttu-id="d0a92-128">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d0a92-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0a92-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0a92-129">Accept</span></span>|<span data-ttu-id="d0a92-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d0a92-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0a92-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a92-131">Request body</span></span>
<span data-ttu-id="d0a92-132">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="d0a92-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="d0a92-133">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="d0a92-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="d0a92-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0a92-134">Property</span></span>|<span data-ttu-id="d0a92-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0a92-135">Type</span></span>|<span data-ttu-id="d0a92-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a92-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0a92-137">id</span><span class="sxs-lookup"><span data-stu-id="d0a92-137">id</span></span>|<span data-ttu-id="d0a92-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0a92-138">String</span></span>|<span data-ttu-id="d0a92-139">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0a92-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="d0a92-140">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="d0a92-140">**On-boarding**</span></span>|
|<span data-ttu-id="d0a92-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="d0a92-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="d0a92-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d0a92-142">Int32</span></span>|<span data-ttu-id="d0a92-143">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="d0a92-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="d0a92-144">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="d0a92-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="d0a92-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0a92-145">Response</span></span>
<span data-ttu-id="d0a92-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune_shared_user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0a92-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0a92-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0a92-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0a92-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a92-148">Request</span></span>
<span data-ttu-id="d0a92-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0a92-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d0a92-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0a92-150">Response</span></span>
<span data-ttu-id="d0a92-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0a92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



