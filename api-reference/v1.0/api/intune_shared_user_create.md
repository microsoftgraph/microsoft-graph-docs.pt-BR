# <a name="create-user"></a><span data-ttu-id="5a7fa-101">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="5a7fa-101">Create user</span></span>

> <span data-ttu-id="5a7fa-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a7fa-103">Criar um novo objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="5a7fa-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a7fa-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a7fa-104">Prerequisites</span></span>
<span data-ttu-id="5a7fa-105">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="5a7fa-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a7fa-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="5a7fa-107">A permissão específica requerida depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="5a7fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a7fa-108">Permission type</span></span>|<span data-ttu-id="5a7fa-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a7fa-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a7fa-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a7fa-110">Delegated (work or school account)</span></span>| <span data-ttu-id="5a7fa-111">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="5a7fa-111">_varies by context_</span></span> |
| <span data-ttu-id="5a7fa-112">&nbsp; &nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="5a7fa-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="5a7fa-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7fa-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5a7fa-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5a7fa-114">.mam</span></span> | <span data-ttu-id="5a7fa-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7fa-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5a7fa-116">&nbsp; &nbsp; Nível de contratação</span><span class="sxs-lookup"><span data-stu-id="5a7fa-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="5a7fa-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7fa-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5a7fa-118">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="5a7fa-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="5a7fa-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7fa-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="5a7fa-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a7fa-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a7fa-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-121">Not supported.</span></span>|
|<span data-ttu-id="5a7fa-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a7fa-122">Application</span></span>|<span data-ttu-id="5a7fa-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a7fa-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a7fa-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="5a7fa-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a7fa-125">Request headers</span></span>
|<span data-ttu-id="5a7fa-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a7fa-126">Header</span></span>|<span data-ttu-id="5a7fa-127">Valor</span><span class="sxs-lookup"><span data-stu-id="5a7fa-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a7fa-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a7fa-128">Authorization</span></span>|<span data-ttu-id="5a7fa-129">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="5a7fa-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a7fa-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a7fa-130">Accept</span></span>|<span data-ttu-id="5a7fa-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5a7fa-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a7fa-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a7fa-132">Request body</span></span>
<span data-ttu-id="5a7fa-133">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="5a7fa-134">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="5a7fa-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a7fa-135">Property</span></span>|<span data-ttu-id="5a7fa-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a7fa-136">Type</span></span>|<span data-ttu-id="5a7fa-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a7fa-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a7fa-138">id</span><span class="sxs-lookup"><span data-stu-id="5a7fa-138">id</span></span>|<span data-ttu-id="5a7fa-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a7fa-139">String</span></span>|<span data-ttu-id="5a7fa-140">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="5a7fa-141">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="5a7fa-141">**On-boarding**</span></span>|
|<span data-ttu-id="5a7fa-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="5a7fa-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="5a7fa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5a7fa-143">Int32</span></span>|<span data-ttu-id="5a7fa-144">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="5a7fa-145">Os valores permitidos são 5 ou 1000.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="5a7fa-146">Suporte de propriedade de corpo de solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="5a7fa-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a7fa-147">Response</span></span>
<span data-ttu-id="5a7fa-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune_shared_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a7fa-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a7fa-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a7fa-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a7fa-150">Request</span></span>
<span data-ttu-id="5a7fa-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="5a7fa-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a7fa-152">Response</span></span>
<span data-ttu-id="5a7fa-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-153">Here is an example of the response.</span></span> <span data-ttu-id="5a7fa-154">Observação: o objeto resposta mostrado aqui pode estar truncado por motivo de concisão.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5a7fa-155">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="5a7fa-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



