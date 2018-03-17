# <a name="list-users"></a><span data-ttu-id="8a1ab-101">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="8a1ab-101">List users</span></span>

> <span data-ttu-id="8a1ab-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a1ab-103">Listar propriedades e relações dos objetos [user](../resources/intune_mam_user.md).</span><span class="sxs-lookup"><span data-stu-id="8a1ab-103">List properties and relationships of the [user](../resources/intune_mam_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a1ab-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a1ab-104">Prerequisites</span></span>
<span data-ttu-id="8a1ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a1ab-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a1ab-107">Permission type</span></span>|<span data-ttu-id="8a1ab-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a1ab-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a1ab-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a1ab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8a1ab-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a1ab-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8a1ab-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a1ab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a1ab-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-112">Not supported.</span></span>|
|<span data-ttu-id="8a1ab-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a1ab-113">Application</span></span>|<span data-ttu-id="8a1ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a1ab-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a1ab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="8a1ab-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ab-116">Request headers</span></span>
|<span data-ttu-id="8a1ab-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a1ab-117">Header</span></span>|<span data-ttu-id="8a1ab-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8a1ab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a1ab-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a1ab-119">Authorization</span></span>|<span data-ttu-id="8a1ab-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a1ab-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a1ab-121">Accept</span></span>|<span data-ttu-id="8a1ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8a1ab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a1ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ab-123">Request body</span></span>
<span data-ttu-id="8a1ab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a1ab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1ab-125">Response</span></span>
<span data-ttu-id="8a1ab-126">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [user](../resources/intune_mam_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-126">If successful, this method returns a `200 OK` response code and collection of [user](../resources/intune_mam_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a1ab-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a1ab-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a1ab-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a1ab-128">Request</span></span>
<span data-ttu-id="8a1ab-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="8a1ab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a1ab-130">Response</span></span>
<span data-ttu-id="8a1ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a1ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



