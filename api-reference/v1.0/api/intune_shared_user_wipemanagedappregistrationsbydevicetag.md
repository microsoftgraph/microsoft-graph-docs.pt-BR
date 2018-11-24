# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="40162-101">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="40162-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="40162-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="40162-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40162-103">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="40162-103">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40162-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40162-104">Prerequisites</span></span>
<span data-ttu-id="40162-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40162-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40162-107">Permission type</span></span>|<span data-ttu-id="40162-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40162-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40162-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40162-109">Delegated (work or school account)</span></span>| <span data-ttu-id="40162-110">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="40162-110">_varies by context_</span></span> |
| <span data-ttu-id="40162-111">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="40162-111">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="40162-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40162-112">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="40162-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40162-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40162-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40162-114">Not supported.</span></span>|
|<span data-ttu-id="40162-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40162-115">Application</span></span>|<span data-ttu-id="40162-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40162-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40162-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40162-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="40162-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40162-118">Request headers</span></span>
|<span data-ttu-id="40162-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40162-119">Header</span></span>|<span data-ttu-id="40162-120">Valor</span><span class="sxs-lookup"><span data-stu-id="40162-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40162-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="40162-121">Authorization</span></span>|<span data-ttu-id="40162-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40162-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40162-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40162-123">Accept</span></span>|<span data-ttu-id="40162-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40162-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40162-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40162-125">Request body</span></span>
<span data-ttu-id="40162-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="40162-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="40162-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="40162-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="40162-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40162-128">Property</span></span>|<span data-ttu-id="40162-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="40162-129">Type</span></span>|<span data-ttu-id="40162-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="40162-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40162-131">deviceTag</span><span class="sxs-lookup"><span data-stu-id="40162-131">deviceTag</span></span>|<span data-ttu-id="40162-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40162-132">String</span></span>|<span data-ttu-id="40162-133">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="40162-133">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="40162-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="40162-134">Response</span></span>
<span data-ttu-id="40162-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40162-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40162-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40162-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="40162-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40162-137">Request</span></span>
<span data-ttu-id="40162-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40162-138">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="40162-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="40162-139">Response</span></span>
<span data-ttu-id="40162-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



