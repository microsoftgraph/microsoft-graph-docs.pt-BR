# <a name="get-managedebookassignment"></a><span data-ttu-id="8c497-101">Obter managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="8c497-101">Get managedEBookAssignment</span></span>

> <span data-ttu-id="8c497-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c497-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c497-103">Ler propriedades e relações do objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c497-103">Read properties and relationships of the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c497-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c497-104">Prerequisites</span></span>
<span data-ttu-id="8c497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c497-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c497-107">Permission type</span></span>|<span data-ttu-id="8c497-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c497-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c497-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c497-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8c497-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c497-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8c497-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c497-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c497-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c497-112">Not supported.</span></span>|
|<span data-ttu-id="8c497-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c497-113">Application</span></span>|<span data-ttu-id="8c497-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c497-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c497-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c497-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c497-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c497-116">Optional query parameters</span></span>
<span data-ttu-id="8c497-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c497-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c497-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c497-118">Request headers</span></span>
|<span data-ttu-id="8c497-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c497-119">Header</span></span>|<span data-ttu-id="8c497-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8c497-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c497-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c497-121">Authorization</span></span>|<span data-ttu-id="8c497-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="8c497-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c497-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c497-123">Accept</span></span>|<span data-ttu-id="8c497-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c497-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c497-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c497-125">Request body</span></span>
<span data-ttu-id="8c497-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c497-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c497-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c497-127">Response</span></span>
<span data-ttu-id="8c497-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c497-128">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c497-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c497-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c497-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c497-130">Request</span></span>
<span data-ttu-id="8c497-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c497-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8c497-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c497-132">Response</span></span>
<span data-ttu-id="8c497-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c497-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```








