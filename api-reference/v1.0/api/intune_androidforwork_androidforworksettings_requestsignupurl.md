# <a name="requestsignupurl-action"></a><span data-ttu-id="6d12e-101">Ação requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="6d12e-101">requestSignupUrl action</span></span>

> <span data-ttu-id="6d12e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d12e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d12e-103">Gera uma URL de inscrição usada para se inscrever no gerenciamento do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="6d12e-103">Generates a sign-up URL that is used to enroll in Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d12e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d12e-104">Prerequisites</span></span>
<span data-ttu-id="6d12e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d12e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6d12e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d12e-107">Permission type</span></span>|<span data-ttu-id="6d12e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d12e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d12e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d12e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6d12e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d12e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d12e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d12e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d12e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d12e-112">Not supported.</span></span>|
|<span data-ttu-id="6d12e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d12e-113">Application</span></span>|<span data-ttu-id="6d12e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d12e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d12e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d12e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="6d12e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d12e-116">Request headers</span></span>
|<span data-ttu-id="6d12e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d12e-117">Header</span></span>|<span data-ttu-id="6d12e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6d12e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d12e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d12e-119">Authorization</span></span>|<span data-ttu-id="6d12e-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d12e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6d12e-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d12e-121">Accept</span></span>|<span data-ttu-id="6d12e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6d12e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d12e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d12e-123">Request body</span></span>
<span data-ttu-id="6d12e-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6d12e-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="6d12e-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6d12e-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6d12e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d12e-126">Property</span></span>|<span data-ttu-id="6d12e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d12e-127">Type</span></span>|<span data-ttu-id="6d12e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d12e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d12e-129">hostName</span><span class="sxs-lookup"><span data-stu-id="6d12e-129">hostname</span></span>|<span data-ttu-id="6d12e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d12e-130">String</span></span>|<span data-ttu-id="6d12e-131">O hostname da URL de retorno de chamada para a qual o navegador será redirecionado depois da conclusão bem-sucedida da inscrição.</span><span class="sxs-lookup"><span data-stu-id="6d12e-131">The hostname of the callback URL to which the browser will be redirected after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="6d12e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d12e-132">Response</span></span>
<span data-ttu-id="6d12e-133">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d12e-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d12e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d12e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d12e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d12e-135">Request</span></span>
<span data-ttu-id="6d12e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d12e-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="6d12e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d12e-137">Response</span></span>
<span data-ttu-id="6d12e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d12e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```



