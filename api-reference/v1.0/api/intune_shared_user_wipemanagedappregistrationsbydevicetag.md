# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="eea38-101">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="eea38-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="eea38-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em versão prévia e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eea38-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eea38-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eea38-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eea38-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eea38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eea38-105">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="eea38-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eea38-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eea38-106">Prerequisites</span></span>
<span data-ttu-id="eea38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eea38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eea38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eea38-109">Permission type</span></span>|<span data-ttu-id="eea38-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eea38-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eea38-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eea38-111">Delegated (work or school account)</span></span>| <span data-ttu-id="eea38-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="eea38-112">_varies by context_</span></span> |
| <span data-ttu-id="eea38-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="eea38-113">.mam</span></span> | <span data-ttu-id="eea38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea38-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="eea38-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eea38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eea38-116">Not supported.</span></span>|
|<span data-ttu-id="eea38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eea38-117">Application</span></span>|<span data-ttu-id="eea38-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eea38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eea38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eea38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="eea38-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eea38-120">Request headers</span></span>
|<span data-ttu-id="eea38-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eea38-121">Header</span></span>|<span data-ttu-id="eea38-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eea38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eea38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eea38-123">Authorization</span></span>|<span data-ttu-id="eea38-124">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="eea38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eea38-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eea38-125">Accept</span></span>|<span data-ttu-id="eea38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eea38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eea38-127">Request body</span></span>
<span data-ttu-id="eea38-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="eea38-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eea38-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="eea38-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eea38-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eea38-130">Property</span></span>|<span data-ttu-id="eea38-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eea38-131">Type</span></span>|<span data-ttu-id="eea38-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea38-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="eea38-133">deviceTag</span></span>|<span data-ttu-id="eea38-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eea38-134">String</span></span>|<span data-ttu-id="eea38-135">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="eea38-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="eea38-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea38-136">Response</span></span>
<span data-ttu-id="eea38-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eea38-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eea38-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eea38-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="eea38-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eea38-139">Request</span></span>
<span data-ttu-id="eea38-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eea38-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="eea38-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea38-141">Response</span></span>
<span data-ttu-id="eea38-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eea38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



