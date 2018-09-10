# <a name="disablelostmode-action"></a><span data-ttu-id="eb775-101">Ação disableLostMode</span><span class="sxs-lookup"><span data-stu-id="eb775-101">disableLostMode action</span></span>

> <span data-ttu-id="eb775-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eb775-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb775-103">Desabilitar o modo perdido</span><span class="sxs-lookup"><span data-stu-id="eb775-103">Disable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb775-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb775-104">Prerequisites</span></span>
<span data-ttu-id="eb775-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb775-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb775-107">Permission type</span></span>|<span data-ttu-id="eb775-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb775-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb775-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb775-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eb775-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="eb775-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="eb775-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb775-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb775-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb775-112">Not supported.</span></span>|
|<span data-ttu-id="eb775-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb775-113">Application</span></span>|<span data-ttu-id="eb775-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb775-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb775-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb775-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="eb775-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb775-116">Request headers</span></span>
|<span data-ttu-id="eb775-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb775-117">Header</span></span>|<span data-ttu-id="eb775-118">Valor</span><span class="sxs-lookup"><span data-stu-id="eb775-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb775-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb775-119">Authorization</span></span>|<span data-ttu-id="eb775-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="eb775-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb775-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb775-121">Accept</span></span>|<span data-ttu-id="eb775-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eb775-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb775-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb775-123">Request body</span></span>
<span data-ttu-id="eb775-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb775-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb775-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb775-125">Response</span></span>
<span data-ttu-id="eb775-126">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb775-126">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eb775-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb775-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb775-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb775-128">Request</span></span>
<span data-ttu-id="eb775-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb775-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="eb775-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb775-130">Response</span></span>
<span data-ttu-id="eb775-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb775-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








