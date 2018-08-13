# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="af12a-101">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="af12a-101">getManagedAppPolicies function</span></span>

> <span data-ttu-id="af12a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af12a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af12a-103">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="af12a-103">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af12a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af12a-104">Prerequisites</span></span>
<span data-ttu-id="af12a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af12a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af12a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af12a-107">Permission type</span></span>|<span data-ttu-id="af12a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af12a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af12a-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af12a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af12a-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="af12a-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="af12a-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af12a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af12a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af12a-112">Not supported.</span></span>|
|<span data-ttu-id="af12a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af12a-113">Application</span></span>|<span data-ttu-id="af12a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af12a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af12a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af12a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="af12a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af12a-116">Request headers</span></span>
|<span data-ttu-id="af12a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af12a-117">Header</span></span>|<span data-ttu-id="af12a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="af12a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af12a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="af12a-119">Authorization</span></span>|<span data-ttu-id="af12a-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af12a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af12a-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af12a-121">Accept</span></span>|<span data-ttu-id="af12a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af12a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af12a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af12a-123">Request body</span></span>
<span data-ttu-id="af12a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af12a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af12a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="af12a-125">Response</span></span>
<span data-ttu-id="af12a-126">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af12a-126">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af12a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af12a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="af12a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af12a-128">Request</span></span>
<span data-ttu-id="af12a-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af12a-129">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="af12a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="af12a-130">Response</span></span>
<span data-ttu-id="af12a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af12a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```



