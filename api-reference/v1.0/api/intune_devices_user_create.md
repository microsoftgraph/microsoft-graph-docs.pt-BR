# <a name="create-user"></a><span data-ttu-id="cf5ee-101">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="cf5ee-101">Create User</span></span>

> <span data-ttu-id="cf5ee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf5ee-103">Criar um novo objeto [user](../resources/intune_devices_user.md).</span><span class="sxs-lookup"><span data-stu-id="cf5ee-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf5ee-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf5ee-104">Prerequisites</span></span>
<span data-ttu-id="cf5ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf5ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf5ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf5ee-107">Permission type</span></span>|<span data-ttu-id="cf5ee-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf5ee-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf5ee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf5ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf5ee-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5ee-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf5ee-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf5ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf5ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-112">Not supported.</span></span>|
|<span data-ttu-id="cf5ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf5ee-113">Application</span></span>|<span data-ttu-id="cf5ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf5ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf5ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="cf5ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5ee-116">Request headers</span></span>
|<span data-ttu-id="cf5ee-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf5ee-117">Header</span></span>|<span data-ttu-id="cf5ee-118">Valor</span><span class="sxs-lookup"><span data-stu-id="cf5ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf5ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf5ee-119">Authorization</span></span>|<span data-ttu-id="cf5ee-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cf5ee-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf5ee-121">Accept</span></span>|<span data-ttu-id="cf5ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cf5ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf5ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5ee-123">Request body</span></span>
<span data-ttu-id="cf5ee-124">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="cf5ee-125">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="cf5ee-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf5ee-126">Property</span></span>|<span data-ttu-id="cf5ee-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf5ee-127">Type</span></span>|<span data-ttu-id="cf5ee-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf5ee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5ee-129">id</span><span class="sxs-lookup"><span data-stu-id="cf5ee-129">id</span></span>|<span data-ttu-id="cf5ee-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf5ee-130">String</span></span>|<span data-ttu-id="cf5ee-131">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-131">Unique identifier for the lab user.</span></span>|



## <a name="response"></a><span data-ttu-id="cf5ee-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5ee-132">Response</span></span>
<span data-ttu-id="cf5ee-133">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune_devices_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-133">If successful, this method returns a `201 Created` response code and [user](../resources/intune_devices_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5ee-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf5ee-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf5ee-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5ee-135">Request</span></span>
<span data-ttu-id="cf5ee-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="cf5ee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5ee-137">Response</span></span>
<span data-ttu-id="cf5ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf5ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



