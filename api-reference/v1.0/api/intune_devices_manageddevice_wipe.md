# <a name="wipe-action"></a><span data-ttu-id="ed2de-101">Ação wipe</span><span class="sxs-lookup"><span data-stu-id="ed2de-101">wipe action</span></span>

> <span data-ttu-id="ed2de-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed2de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed2de-103">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed2de-103">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed2de-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed2de-104">Prerequisites</span></span>
<span data-ttu-id="ed2de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed2de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ed2de-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed2de-107">Permission type</span></span>|<span data-ttu-id="ed2de-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed2de-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed2de-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed2de-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ed2de-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ed2de-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ed2de-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed2de-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed2de-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed2de-112">Not supported.</span></span>|
|<span data-ttu-id="ed2de-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed2de-113">Application</span></span>|<span data-ttu-id="ed2de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed2de-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed2de-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed2de-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="ed2de-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed2de-116">Request headers</span></span>
|<span data-ttu-id="ed2de-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed2de-117">Header</span></span>|<span data-ttu-id="ed2de-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ed2de-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed2de-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed2de-119">Authorization</span></span>|<span data-ttu-id="ed2de-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ed2de-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed2de-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed2de-121">Accept</span></span>|<span data-ttu-id="ed2de-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ed2de-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed2de-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed2de-123">Request body</span></span>
<span data-ttu-id="ed2de-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ed2de-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ed2de-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ed2de-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ed2de-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed2de-126">Property</span></span>|<span data-ttu-id="ed2de-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed2de-127">Type</span></span>|<span data-ttu-id="ed2de-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed2de-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed2de-129">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="ed2de-129">keepEnrollmentData</span></span>|<span data-ttu-id="ed2de-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed2de-130">Boolean</span></span>|<span data-ttu-id="ed2de-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed2de-131">Not yet documented</span></span>|
|<span data-ttu-id="ed2de-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="ed2de-132">keepUserData</span></span>|<span data-ttu-id="ed2de-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed2de-133">Boolean</span></span>|<span data-ttu-id="ed2de-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed2de-134">Not yet documented</span></span>|
|<span data-ttu-id="ed2de-135">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="ed2de-135">macOsUnlockCode</span></span>|<span data-ttu-id="ed2de-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed2de-136">String</span></span>|<span data-ttu-id="ed2de-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed2de-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ed2de-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed2de-138">Response</span></span>
<span data-ttu-id="ed2de-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed2de-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed2de-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed2de-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed2de-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed2de-141">Request</span></span>
<span data-ttu-id="ed2de-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed2de-142">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe
Content-type: application/json

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="ed2de-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed2de-143">Response</span></span>
<span data-ttu-id="ed2de-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed2de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "response" } -->
``` http
HTTP/1.1 204 No Content
```



