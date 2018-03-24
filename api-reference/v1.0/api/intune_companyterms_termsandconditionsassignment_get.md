# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="6def7-101">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6def7-101">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="6def7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6def7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6def7-103">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6def7-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6def7-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6def7-104">Prerequisites</span></span>
<span data-ttu-id="6def7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6def7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6def7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6def7-107">Permission type</span></span>|<span data-ttu-id="6def7-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6def7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6def7-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6def7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6def7-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6def7-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6def7-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6def7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6def7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6def7-112">Not supported.</span></span>|
|<span data-ttu-id="6def7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6def7-113">Application</span></span>|<span data-ttu-id="6def7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6def7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6def7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6def7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6def7-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6def7-116">Optional query parameters</span></span>
<span data-ttu-id="6def7-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6def7-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6def7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6def7-118">Request headers</span></span>
|<span data-ttu-id="6def7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6def7-119">Header</span></span>|<span data-ttu-id="6def7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6def7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6def7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6def7-121">Authorization</span></span>|<span data-ttu-id="6def7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6def7-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6def7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6def7-123">Accept</span></span>|<span data-ttu-id="6def7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6def7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6def7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6def7-125">Request body</span></span>
<span data-ttu-id="6def7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6def7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6def7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6def7-127">Response</span></span>
<span data-ttu-id="6def7-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6def7-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_companyterms_termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6def7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6def7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6def7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6def7-130">Request</span></span>
<span data-ttu-id="6def7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6def7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6def7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6def7-132">Response</span></span>
<span data-ttu-id="6def7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6def7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



