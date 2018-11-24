# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="61266-101">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="61266-101">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="61266-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61266-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61266-103">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="61266-103">Delete user from shared Apple device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61266-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61266-104">Prerequisites</span></span>
<span data-ttu-id="61266-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61266-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61266-107">Permission type</span></span>|<span data-ttu-id="61266-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61266-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61266-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61266-109">Delegated (work or school account)</span></span>|<span data-ttu-id="61266-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="61266-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="61266-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61266-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61266-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61266-112">Not supported.</span></span>|
|<span data-ttu-id="61266-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61266-113">Application</span></span>|<span data-ttu-id="61266-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61266-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61266-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61266-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="61266-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61266-116">Request headers</span></span>
|<span data-ttu-id="61266-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61266-117">Header</span></span>|<span data-ttu-id="61266-118">Valor</span><span class="sxs-lookup"><span data-stu-id="61266-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61266-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="61266-119">Authorization</span></span>|<span data-ttu-id="61266-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61266-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61266-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61266-121">Accept</span></span>|<span data-ttu-id="61266-122">application/json</span><span class="sxs-lookup"><span data-stu-id="61266-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61266-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61266-123">Request body</span></span>
<span data-ttu-id="61266-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="61266-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="61266-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="61266-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="61266-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61266-126">Property</span></span>|<span data-ttu-id="61266-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="61266-127">Type</span></span>|<span data-ttu-id="61266-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="61266-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61266-129">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="61266-129">userPrincipalName</span></span>|<span data-ttu-id="61266-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61266-130">String</span></span>|<span data-ttu-id="61266-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61266-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="61266-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="61266-132">Response</span></span>
<span data-ttu-id="61266-133">Se tiver êxito, esta ação retornará o código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="61266-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61266-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61266-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="61266-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61266-135">Request</span></span>
<span data-ttu-id="61266-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61266-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="61266-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="61266-137">Response</span></span>
<span data-ttu-id="61266-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61266-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



