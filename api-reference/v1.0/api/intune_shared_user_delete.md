# <a name="delete-user"></a><span data-ttu-id="14f29-101">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="14f29-101">Delete user</span></span>

> <span data-ttu-id="14f29-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="14f29-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14f29-103">Exclui [usuário](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="14f29-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14f29-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14f29-104">Prerequisites</span></span>
<span data-ttu-id="14f29-105">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="14f29-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="14f29-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14f29-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="14f29-107">A permissão específica necessária depende de contexto.</span><span class="sxs-lookup"><span data-stu-id="14f29-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="14f29-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14f29-108">Permission type</span></span>|<span data-ttu-id="14f29-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14f29-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14f29-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14f29-110">Delegated (work or school account)</span></span>| <span data-ttu-id="14f29-111">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="14f29-111">_varies by context_</span></span>|
| <span data-ttu-id="14f29-112">&nbsp;&nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="14f29-112">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="14f29-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f29-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="14f29-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="14f29-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="14f29-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f29-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="14f29-116">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="14f29-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="14f29-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f29-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="14f29-118">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="14f29-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="14f29-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f29-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="14f29-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14f29-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14f29-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14f29-121">Not supported.</span></span>|
|<span data-ttu-id="14f29-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14f29-122">Application</span></span>|<span data-ttu-id="14f29-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14f29-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14f29-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14f29-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="14f29-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14f29-125">Request headers</span></span>
|<span data-ttu-id="14f29-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14f29-126">Header</span></span>|<span data-ttu-id="14f29-127">Valor</span><span class="sxs-lookup"><span data-stu-id="14f29-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14f29-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="14f29-128">Authorization</span></span>|<span data-ttu-id="14f29-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14f29-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14f29-130">Accept</span><span class="sxs-lookup"><span data-stu-id="14f29-130">Accept</span></span>|<span data-ttu-id="14f29-131">application/json</span><span class="sxs-lookup"><span data-stu-id="14f29-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14f29-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14f29-132">Request body</span></span>
<span data-ttu-id="14f29-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14f29-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14f29-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14f29-134">Response</span></span>
<span data-ttu-id="14f29-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14f29-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14f29-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14f29-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="14f29-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14f29-137">Request</span></span>
<span data-ttu-id="14f29-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14f29-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="14f29-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="14f29-139">Response</span></span>
<span data-ttu-id="14f29-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14f29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



