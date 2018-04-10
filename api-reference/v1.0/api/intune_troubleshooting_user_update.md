# <a name="update-user"></a><span data-ttu-id="b3802-101">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="b3802-101">Update user</span></span>

> <span data-ttu-id="b3802-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3802-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3802-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3802-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3802-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3802-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3802-105">Atualizar as propriedades de um objeto [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-105">Update the properties of a [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3802-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3802-106">Prerequisites</span></span>
<span data-ttu-id="b3802-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3802-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3802-109">Permission type</span></span>|<span data-ttu-id="b3802-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3802-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3802-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3802-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3802-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3802-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b3802-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3802-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3802-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3802-114">Not supported.</span></span>|
|<span data-ttu-id="b3802-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3802-115">Application</span></span>|<span data-ttu-id="b3802-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3802-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3802-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3802-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="b3802-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-118">Request headers</span></span>
|<span data-ttu-id="b3802-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3802-119">Header</span></span>|<span data-ttu-id="b3802-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b3802-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3802-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3802-121">Authorization</span></span>|<span data-ttu-id="b3802-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3802-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3802-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3802-123">Accept</span></span>|<span data-ttu-id="b3802-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3802-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3802-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-125">Request body</span></span>
<span data-ttu-id="b3802-126">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-126">In the request body, supply a JSON representation for the [user](../resources/intune_troubleshooting_user.md) object.</span></span>

<span data-ttu-id="b3802-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-127">The following table shows the properties that are required when you create the [user](../resources/intune_troubleshooting_user.md).</span></span>

|<span data-ttu-id="b3802-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3802-128">Property</span></span>|<span data-ttu-id="b3802-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3802-129">Type</span></span>|<span data-ttu-id="b3802-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3802-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3802-131">id</span><span class="sxs-lookup"><span data-stu-id="b3802-131">id</span></span>|<span data-ttu-id="b3802-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3802-132">String</span></span>|<span data-ttu-id="b3802-133">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b3802-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="b3802-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3802-134">Response</span></span>
<span data-ttu-id="b3802-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune_troubleshooting_user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3802-135">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3802-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3802-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3802-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-137">Request</span></span>
<span data-ttu-id="b3802-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3802-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b3802-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3802-139">Response</span></span>
<span data-ttu-id="b3802-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3802-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



