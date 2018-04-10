# <a name="list-users"></a><span data-ttu-id="bc99d-101">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="bc99d-101">List users</span></span>

> <span data-ttu-id="bc99d-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc99d-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc99d-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc99d-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc99d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc99d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc99d-105">Listar propriedades e relações de objetos de [usuário](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="bc99d-105">List properties and relationships of the [user](../resources/intune_troubleshooting_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc99d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc99d-106">Prerequisites</span></span>
<span data-ttu-id="bc99d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc99d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc99d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc99d-109">Permission type</span></span>|<span data-ttu-id="bc99d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc99d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc99d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc99d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc99d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc99d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bc99d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc99d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc99d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc99d-114">Not supported.</span></span>|
|<span data-ttu-id="bc99d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc99d-115">Application</span></span>|<span data-ttu-id="bc99d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc99d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc99d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc99d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="bc99d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99d-118">Request headers</span></span>
|<span data-ttu-id="bc99d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc99d-119">Header</span></span>|<span data-ttu-id="bc99d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bc99d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc99d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc99d-121">Authorization</span></span>|<span data-ttu-id="bc99d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc99d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc99d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc99d-123">Accept</span></span>|<span data-ttu-id="bc99d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc99d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc99d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99d-125">Request body</span></span>
<span data-ttu-id="bc99d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc99d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc99d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc99d-127">Response</span></span>
<span data-ttu-id="bc99d-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune_troubleshooting_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc99d-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_troubleshooting_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc99d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc99d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc99d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc99d-130">Request</span></span>
<span data-ttu-id="bc99d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc99d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="bc99d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc99d-132">Response</span></span>
<span data-ttu-id="bc99d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc99d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



