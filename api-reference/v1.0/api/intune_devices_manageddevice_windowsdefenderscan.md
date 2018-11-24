# <a name="windowsdefenderscan-action"></a><span data-ttu-id="01e0d-101">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="01e0d-101">windowsDefenderScan action</span></span>

> <span data-ttu-id="01e0d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01e0d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01e0d-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01e0d-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01e0d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01e0d-104">Prerequisites</span></span>
<span data-ttu-id="01e0d-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01e0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01e0d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01e0d-107">Permission type</span></span>|<span data-ttu-id="01e0d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01e0d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01e0d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01e0d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01e0d-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="01e0d-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="01e0d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01e0d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01e0d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01e0d-112">Not supported.</span></span>|
|<span data-ttu-id="01e0d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01e0d-113">Application</span></span>|<span data-ttu-id="01e0d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01e0d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01e0d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01e0d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="01e0d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01e0d-116">Request headers</span></span>
|<span data-ttu-id="01e0d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01e0d-117">Header</span></span>|<span data-ttu-id="01e0d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="01e0d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01e0d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="01e0d-119">Authorization</span></span>|<span data-ttu-id="01e0d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01e0d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01e0d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01e0d-121">Accept</span></span>|<span data-ttu-id="01e0d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01e0d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e0d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01e0d-123">Request body</span></span>
<span data-ttu-id="01e0d-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="01e0d-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="01e0d-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="01e0d-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="01e0d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01e0d-126">Property</span></span>|<span data-ttu-id="01e0d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="01e0d-127">Type</span></span>|<span data-ttu-id="01e0d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="01e0d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01e0d-129">quickScan</span><span class="sxs-lookup"><span data-stu-id="01e0d-129">quickScan</span></span>|<span data-ttu-id="01e0d-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="01e0d-130">Boolean</span></span>|<span data-ttu-id="01e0d-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01e0d-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="01e0d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e0d-132">Response</span></span>
<span data-ttu-id="01e0d-133">Se tiver êxito, esta ação retornará o código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01e0d-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01e0d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01e0d-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="01e0d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01e0d-135">Request</span></span>
<span data-ttu-id="01e0d-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01e0d-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="01e0d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e0d-137">Response</span></span>
<span data-ttu-id="01e0d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01e0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



