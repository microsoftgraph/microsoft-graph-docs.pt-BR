# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="339b5-101">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="339b5-101">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="339b5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="339b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="339b5-103">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="339b5-103">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="339b5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="339b5-104">Prerequisites</span></span>
<span data-ttu-id="339b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="339b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="339b5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="339b5-107">Permission type</span></span>|<span data-ttu-id="339b5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="339b5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="339b5-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="339b5-109">Delegated (work or school account)</span></span>| <span data-ttu-id="339b5-110">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="339b5-110">_varies by context_</span></span> |
| <span data-ttu-id="339b5-111">&nbsp; &nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="339b5-111">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="339b5-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="339b5-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="339b5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="339b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="339b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="339b5-114">Not supported.</span></span>|
|<span data-ttu-id="339b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="339b5-115">Application</span></span>|<span data-ttu-id="339b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="339b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="339b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="339b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="339b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="339b5-118">Request headers</span></span>
|<span data-ttu-id="339b5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="339b5-119">Header</span></span>|<span data-ttu-id="339b5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="339b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="339b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="339b5-121">Authorization</span></span>|<span data-ttu-id="339b5-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="339b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="339b5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="339b5-123">Accept</span></span>|<span data-ttu-id="339b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="339b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="339b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="339b5-125">Request body</span></span>
<span data-ttu-id="339b5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="339b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="339b5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="339b5-127">Response</span></span>
<span data-ttu-id="339b5-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="339b5-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="339b5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="339b5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="339b5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="339b5-130">Request</span></span>
<span data-ttu-id="339b5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="339b5-131">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="339b5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="339b5-132">Response</span></span>
<span data-ttu-id="339b5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="339b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



