# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="c5d3f-101">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="c5d3f-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="c5d3f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5d3f-103">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5d3f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5d3f-104">Prerequisites</span></span>
<span data-ttu-id="c5d3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5d3f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5d3f-107">Permission type</span></span>|<span data-ttu-id="c5d3f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5d3f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d3f-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5d3f-109">Delegated (work or school account)</span></span>| <span data-ttu-id="c5d3f-110">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="c5d3f-110">_varies by context_</span></span>|
| <span data-ttu-id="c5d3f-111">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c5d3f-111">.mam</span></span> | <span data-ttu-id="c5d3f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5d3f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="c5d3f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5d3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d3f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-114">Not supported.</span></span>|
|<span data-ttu-id="c5d3f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5d3f-115">Application</span></span>|<span data-ttu-id="c5d3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d3f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5d3f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c5d3f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3f-118">Request headers</span></span>
|<span data-ttu-id="c5d3f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5d3f-119">Header</span></span>|<span data-ttu-id="c5d3f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c5d3f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d3f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5d3f-121">Authorization</span></span>|<span data-ttu-id="c5d3f-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="c5d3f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d3f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5d3f-123">Accept</span></span>|<span data-ttu-id="c5d3f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d3f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d3f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3f-125">Request body</span></span>
<span data-ttu-id="c5d3f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5d3f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d3f-127">Response</span></span>
<span data-ttu-id="c5d3f-128">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-128">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d3f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5d3f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d3f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d3f-130">Request</span></span>
<span data-ttu-id="c5d3f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-131">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="c5d3f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d3f-132">Response</span></span>
<span data-ttu-id="c5d3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5d3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



