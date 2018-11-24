# <a name="create-user"></a><span data-ttu-id="cdaae-101">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="cdaae-101">Create user</span></span>

> <span data-ttu-id="cdaae-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cdaae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdaae-103">Criar um novo objeto [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="cdaae-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdaae-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdaae-104">Prerequisites</span></span>
<span data-ttu-id="cdaae-105">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cdaae-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cdaae-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cdaae-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="cdaae-107">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="cdaae-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="cdaae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdaae-108">Permission type</span></span>|<span data-ttu-id="cdaae-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdaae-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdaae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdaae-110">Delegated (work or school account)</span></span>| <span data-ttu-id="cdaae-111">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="cdaae-111">_varies by context_</span></span> |
| <span data-ttu-id="cdaae-112">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cdaae-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="cdaae-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdaae-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cdaae-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="cdaae-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="cdaae-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdaae-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cdaae-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="cdaae-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="cdaae-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdaae-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cdaae-118">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="cdaae-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="cdaae-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdaae-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="cdaae-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdaae-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdaae-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdaae-121">Not supported.</span></span>|
|<span data-ttu-id="cdaae-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdaae-122">Application</span></span>|<span data-ttu-id="cdaae-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdaae-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdaae-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdaae-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="cdaae-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdaae-125">Request headers</span></span>
|<span data-ttu-id="cdaae-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdaae-126">Header</span></span>|<span data-ttu-id="cdaae-127">Valor</span><span class="sxs-lookup"><span data-stu-id="cdaae-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdaae-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdaae-128">Authorization</span></span>|<span data-ttu-id="cdaae-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdaae-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdaae-130">Accept</span><span class="sxs-lookup"><span data-stu-id="cdaae-130">Accept</span></span>|<span data-ttu-id="cdaae-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cdaae-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdaae-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdaae-132">Request body</span></span>
<span data-ttu-id="cdaae-133">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="cdaae-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="cdaae-134">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="cdaae-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="cdaae-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdaae-135">Property</span></span>|<span data-ttu-id="cdaae-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdaae-136">Type</span></span>|<span data-ttu-id="cdaae-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdaae-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdaae-138">id</span><span class="sxs-lookup"><span data-stu-id="cdaae-138">id</span></span>|<span data-ttu-id="cdaae-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdaae-139">String</span></span>|<span data-ttu-id="cdaae-140">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="cdaae-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="cdaae-141">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="cdaae-141">**Onboarding**</span></span>|
|<span data-ttu-id="cdaae-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="cdaae-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="cdaae-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaae-143">Int32</span></span>|<span data-ttu-id="cdaae-144">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="cdaae-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="cdaae-145">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="cdaae-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="cdaae-146">Suporte de propriedade de corpo de solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="cdaae-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="cdaae-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdaae-147">Response</span></span>
<span data-ttu-id="cdaae-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune_shared_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdaae-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdaae-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdaae-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdaae-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdaae-150">Request</span></span>
<span data-ttu-id="cdaae-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdaae-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="cdaae-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdaae-152">Response</span></span>
<span data-ttu-id="cdaae-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdaae-153">Here is an example of the response.</span></span> <span data-ttu-id="cdaae-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cdaae-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdaae-155">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="cdaae-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



