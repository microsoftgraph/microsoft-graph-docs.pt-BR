# <a name="update-user"></a><span data-ttu-id="9d60b-101">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="9d60b-101">Update user</span></span>

> <span data-ttu-id="9d60b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9d60b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d60b-103">Atualizar as propriedades de um objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="9d60b-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d60b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d60b-104">Prerequisites</span></span>
<span data-ttu-id="9d60b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d60b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d60b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d60b-107">Permission type</span></span>|<span data-ttu-id="9d60b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d60b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d60b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d60b-109">Delegated (work or school account)</span></span>| <span data-ttu-id="9d60b-110">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="9d60b-110">_varies by context_</span></span>|
| <span data-ttu-id="9d60b-111">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="9d60b-111">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9d60b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d60b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9d60b-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9d60b-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="9d60b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d60b-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9d60b-115">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="9d60b-115">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9d60b-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d60b-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9d60b-117">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="9d60b-117">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9d60b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d60b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="9d60b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d60b-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d60b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d60b-120">Not supported.</span></span>|
|<span data-ttu-id="9d60b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d60b-121">Application</span></span>|<span data-ttu-id="9d60b-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d60b-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d60b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d60b-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="9d60b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d60b-124">Request headers</span></span>
|<span data-ttu-id="9d60b-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d60b-125">Header</span></span>|<span data-ttu-id="9d60b-126">Valor</span><span class="sxs-lookup"><span data-stu-id="9d60b-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d60b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d60b-127">Authorization</span></span>|<span data-ttu-id="9d60b-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d60b-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d60b-129">Accept</span><span class="sxs-lookup"><span data-stu-id="9d60b-129">Accept</span></span>|<span data-ttu-id="9d60b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9d60b-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d60b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d60b-131">Request body</span></span>
<span data-ttu-id="9d60b-132">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="9d60b-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="9d60b-133">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="9d60b-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="9d60b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d60b-134">Property</span></span>|<span data-ttu-id="9d60b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d60b-135">Type</span></span>|<span data-ttu-id="9d60b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d60b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d60b-137">id</span><span class="sxs-lookup"><span data-stu-id="9d60b-137">id</span></span>|<span data-ttu-id="9d60b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d60b-138">String</span></span>|<span data-ttu-id="9d60b-139">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="9d60b-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="9d60b-140">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="9d60b-140">**Onboarding**</span></span>|
|<span data-ttu-id="9d60b-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="9d60b-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="9d60b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9d60b-142">Int32</span></span>|<span data-ttu-id="9d60b-143">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="9d60b-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="9d60b-144">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="9d60b-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="9d60b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d60b-145">Response</span></span>
<span data-ttu-id="9d60b-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune_shared_user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d60b-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d60b-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d60b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d60b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d60b-148">Request</span></span>
<span data-ttu-id="9d60b-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d60b-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="9d60b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d60b-150">Response</span></span>
<span data-ttu-id="9d60b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d60b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



