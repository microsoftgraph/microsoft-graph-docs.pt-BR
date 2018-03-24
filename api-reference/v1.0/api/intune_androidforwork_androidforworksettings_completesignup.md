# <a name="completesignup-action"></a><span data-ttu-id="2ea9c-101">Ação completeSignup</span><span class="sxs-lookup"><span data-stu-id="2ea9c-101">completeSignup action</span></span>

> <span data-ttu-id="2ea9c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ea9c-103">Conclui o fluxo de inscrição para gerenciamento do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-103">Completes the sign-up flow for Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ea9c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ea9c-104">Prerequisites</span></span>
<span data-ttu-id="2ea9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ea9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ea9c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ea9c-107">Permission type</span></span>|<span data-ttu-id="2ea9c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ea9c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ea9c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ea9c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2ea9c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ea9c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ea9c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ea9c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ea9c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-112">Not supported.</span></span>|
|<span data-ttu-id="2ea9c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ea9c-113">Application</span></span>|<span data-ttu-id="2ea9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ea9c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea9c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="2ea9c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea9c-116">Request headers</span></span>
|<span data-ttu-id="2ea9c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ea9c-117">Header</span></span>|<span data-ttu-id="2ea9c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2ea9c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ea9c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ea9c-119">Authorization</span></span>|<span data-ttu-id="2ea9c-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ea9c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ea9c-121">Accept</span></span>|<span data-ttu-id="2ea9c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2ea9c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ea9c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea9c-123">Request body</span></span>
<span data-ttu-id="2ea9c-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="2ea9c-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2ea9c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ea9c-126">Property</span></span>|<span data-ttu-id="2ea9c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ea9c-127">Type</span></span>|<span data-ttu-id="2ea9c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ea9c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea9c-129">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="2ea9c-129">enterpriseToken</span></span>|<span data-ttu-id="2ea9c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ea9c-130">String</span></span>|<span data-ttu-id="2ea9c-131">O token do Enterprise anexado à URL de retorno de chamada depois da conclusão bem-sucedida da inscrição.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-131">The Enterprise token appended to the callback URL after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="2ea9c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ea9c-132">Response</span></span>
<span data-ttu-id="2ea9c-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ea9c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ea9c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ea9c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ea9c-135">Request</span></span>
<span data-ttu-id="2ea9c-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="2ea9c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ea9c-137">Response</span></span>
<span data-ttu-id="2ea9c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ea9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



