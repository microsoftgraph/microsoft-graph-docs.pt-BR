# <a name="update-user"></a><span data-ttu-id="a6875-101">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="a6875-101">Update user</span></span>

> <span data-ttu-id="a6875-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6875-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6875-103">Atualizar as propriedades de um objeto [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="a6875-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6875-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6875-104">Prerequisites</span></span>
<span data-ttu-id="a6875-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6875-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6875-107">Permission type</span></span>|<span data-ttu-id="a6875-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6875-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6875-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6875-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a6875-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6875-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6875-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6875-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6875-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6875-112">Not supported.</span></span>|
|<span data-ttu-id="a6875-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6875-113">Application</span></span>|<span data-ttu-id="a6875-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6875-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6875-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6875-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="a6875-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6875-116">Request headers</span></span>
|<span data-ttu-id="a6875-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6875-117">Header</span></span>|<span data-ttu-id="a6875-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a6875-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6875-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6875-119">Authorization</span></span>|<span data-ttu-id="a6875-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6875-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6875-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6875-121">Accept</span></span>|<span data-ttu-id="a6875-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a6875-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6875-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6875-123">Request body</span></span>
<span data-ttu-id="a6875-124">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="a6875-124">In the request body, supply a JSON representation of [user](../resources/intune_onboarding_user.md) object.</span></span>

<span data-ttu-id="a6875-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="a6875-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a6875-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6875-126">Property</span></span>|<span data-ttu-id="a6875-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6875-127">Type</span></span>|<span data-ttu-id="a6875-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6875-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6875-129">id</span><span class="sxs-lookup"><span data-stu-id="a6875-129">id</span></span>|<span data-ttu-id="a6875-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6875-130">String</span></span>|<span data-ttu-id="a6875-131">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="a6875-131">Unique identifier for the lab user.</span></span>|
|<span data-ttu-id="a6875-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="a6875-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="a6875-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a6875-133">Int32</span></span>|<span data-ttu-id="a6875-134">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="a6875-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="a6875-135">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="a6875-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="a6875-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6875-136">Response</span></span>
<span data-ttu-id="a6875-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune_onboarding_user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6875-137">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6875-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6875-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6875-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6875-139">Request</span></span>
<span data-ttu-id="a6875-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6875-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 34

{
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="a6875-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6875-141">Response</span></span>
<span data-ttu-id="a6875-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6875-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



