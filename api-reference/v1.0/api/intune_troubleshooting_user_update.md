# <a name="update-user"></a><span data-ttu-id="57444-101">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="57444-101">Update user</span></span>

> <span data-ttu-id="57444-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57444-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57444-103">Atualizar as propriedades de um objeto [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="57444-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57444-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57444-104">Prerequisites</span></span>
<span data-ttu-id="57444-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57444-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57444-107">Permission type</span></span>|<span data-ttu-id="57444-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57444-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57444-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57444-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57444-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57444-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57444-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57444-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57444-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57444-112">Not supported.</span></span>|
|<span data-ttu-id="57444-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57444-113">Application</span></span>|<span data-ttu-id="57444-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57444-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57444-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57444-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="57444-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57444-116">Request headers</span></span>
|<span data-ttu-id="57444-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57444-117">Header</span></span>|<span data-ttu-id="57444-118">Valor</span><span class="sxs-lookup"><span data-stu-id="57444-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57444-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="57444-119">Authorization</span></span>|<span data-ttu-id="57444-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57444-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57444-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57444-121">Accept</span></span>|<span data-ttu-id="57444-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57444-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57444-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57444-123">Request body</span></span>
<span data-ttu-id="57444-124">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="57444-124">In the request body, supply a JSON representation of [user](../resources/intune_troubleshooting_user.md) object.</span></span>

<span data-ttu-id="57444-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="57444-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="57444-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57444-126">Property</span></span>|<span data-ttu-id="57444-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="57444-127">Type</span></span>|<span data-ttu-id="57444-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="57444-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57444-129">id</span><span class="sxs-lookup"><span data-stu-id="57444-129">id</span></span>|<span data-ttu-id="57444-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57444-130">String</span></span>|<span data-ttu-id="57444-131">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="57444-131">Unique identifier for the lab user.</span></span>|



## <a name="response"></a><span data-ttu-id="57444-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="57444-132">Response</span></span>
<span data-ttu-id="57444-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune_troubleshooting_user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57444-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57444-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57444-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="57444-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57444-135">Request</span></span>
<span data-ttu-id="57444-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57444-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="57444-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="57444-137">Response</span></span>
<span data-ttu-id="57444-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57444-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



