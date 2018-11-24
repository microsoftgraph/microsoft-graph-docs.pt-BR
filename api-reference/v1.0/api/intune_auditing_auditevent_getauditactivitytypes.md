# <a name="getauditactivitytypes-function"></a><span data-ttu-id="a6519-101">Função getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="a6519-101">getAuditActivityTypes function</span></span>

> <span data-ttu-id="a6519-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6519-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6519-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6519-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6519-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6519-104">Prerequisites</span></span>
<span data-ttu-id="a6519-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6519-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6519-107">Permission type</span></span>|<span data-ttu-id="a6519-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6519-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6519-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6519-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a6519-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6519-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6519-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6519-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6519-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6519-112">Not supported.</span></span>|
|<span data-ttu-id="a6519-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6519-113">Application</span></span>|<span data-ttu-id="a6519-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6519-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6519-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6519-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="a6519-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6519-116">Request headers</span></span>
|<span data-ttu-id="a6519-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6519-117">Header</span></span>|<span data-ttu-id="a6519-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a6519-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6519-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6519-119">Authorization</span></span>|<span data-ttu-id="a6519-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6519-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6519-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6519-121">Accept</span></span>|<span data-ttu-id="a6519-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a6519-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6519-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6519-123">Request body</span></span>
<span data-ttu-id="a6519-124">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="a6519-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a6519-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a6519-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a6519-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6519-126">Property</span></span>|<span data-ttu-id="a6519-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6519-127">Type</span></span>|<span data-ttu-id="a6519-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6519-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6519-129">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="a6519-129">category</span></span>|<span data-ttu-id="a6519-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6519-130">String</span></span>|<span data-ttu-id="a6519-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6519-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6519-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6519-132">Response</span></span>
<span data-ttu-id="a6519-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6519-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6519-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6519-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6519-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6519-135">Request</span></span>
<span data-ttu-id="a6519-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6519-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a6519-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6519-137">Response</span></span>
<span data-ttu-id="a6519-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6519-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



