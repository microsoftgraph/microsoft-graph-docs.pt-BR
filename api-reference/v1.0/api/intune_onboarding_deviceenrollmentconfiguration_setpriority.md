# <a name="setpriority-action"></a><span data-ttu-id="74bf1-101">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="74bf1-101">setPriority action</span></span>

> <span data-ttu-id="74bf1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74bf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74bf1-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf1-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74bf1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74bf1-104">Prerequisites</span></span>
<span data-ttu-id="74bf1-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="74bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74bf1-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74bf1-107">Permission type</span></span>|<span data-ttu-id="74bf1-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74bf1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74bf1-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74bf1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="74bf1-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74bf1-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74bf1-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74bf1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74bf1-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74bf1-112">Not supported.</span></span>|
|<span data-ttu-id="74bf1-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74bf1-113">Application</span></span>|<span data-ttu-id="74bf1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74bf1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74bf1-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74bf1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="74bf1-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf1-116">Request headers</span></span>
|<span data-ttu-id="74bf1-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74bf1-117">Header</span></span>|<span data-ttu-id="74bf1-118">Valor</span><span class="sxs-lookup"><span data-stu-id="74bf1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74bf1-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="74bf1-119">Authorization</span></span>|<span data-ttu-id="74bf1-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74bf1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="74bf1-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74bf1-121">Accept</span></span>|<span data-ttu-id="74bf1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="74bf1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74bf1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf1-123">Request body</span></span>
<span data-ttu-id="74bf1-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="74bf1-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="74bf1-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="74bf1-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="74bf1-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74bf1-126">Property</span></span>|<span data-ttu-id="74bf1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="74bf1-127">Type</span></span>|<span data-ttu-id="74bf1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="74bf1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74bf1-129">Prioridade</span><span class="sxs-lookup"><span data-stu-id="74bf1-129">priority</span></span>|<span data-ttu-id="74bf1-130">Int32</span><span class="sxs-lookup"><span data-stu-id="74bf1-130">Int32</span></span>|<span data-ttu-id="74bf1-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="74bf1-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="74bf1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bf1-132">Response</span></span>
<span data-ttu-id="74bf1-133">Se tiver êxito, esta ação retornará o código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74bf1-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74bf1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74bf1-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="74bf1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74bf1-135">Request</span></span>
<span data-ttu-id="74bf1-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74bf1-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="74bf1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bf1-137">Response</span></span>
<span data-ttu-id="74bf1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74bf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



