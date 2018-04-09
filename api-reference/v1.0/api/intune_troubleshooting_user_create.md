# <a name="create-user"></a><span data-ttu-id="6463f-101">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="6463f-101">Create user</span></span>

> <span data-ttu-id="6463f-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6463f-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6463f-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6463f-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6463f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6463f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6463f-105">Criar um novo objeto [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="6463f-105">Create a new [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6463f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6463f-106">Prerequisites</span></span>
<span data-ttu-id="6463f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6463f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6463f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6463f-109">Permission type</span></span>|<span data-ttu-id="6463f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6463f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6463f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6463f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6463f-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6463f-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6463f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6463f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6463f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6463f-114">Not supported.</span></span>|
|<span data-ttu-id="6463f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6463f-115">Application</span></span>|<span data-ttu-id="6463f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6463f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6463f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6463f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="6463f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6463f-118">Request headers</span></span>
|<span data-ttu-id="6463f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6463f-119">Header</span></span>|<span data-ttu-id="6463f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6463f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6463f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6463f-121">Authorization</span></span>|<span data-ttu-id="6463f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6463f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6463f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6463f-123">Accept</span></span>|<span data-ttu-id="6463f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6463f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6463f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6463f-125">Request body</span></span>
<span data-ttu-id="6463f-126">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="6463f-126">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="6463f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="6463f-127">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="6463f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6463f-128">Property</span></span>|<span data-ttu-id="6463f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6463f-129">Type</span></span>|<span data-ttu-id="6463f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6463f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6463f-131">id</span><span class="sxs-lookup"><span data-stu-id="6463f-131">id</span></span>|<span data-ttu-id="6463f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6463f-132">String</span></span>|<span data-ttu-id="6463f-133">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6463f-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="6463f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6463f-134">Response</span></span>
<span data-ttu-id="6463f-135">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune_troubleshooting_user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6463f-135">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6463f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6463f-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="6463f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6463f-137">Request</span></span>
<span data-ttu-id="6463f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6463f-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="6463f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6463f-139">Response</span></span>
<span data-ttu-id="6463f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6463f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



