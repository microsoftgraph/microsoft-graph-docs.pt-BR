# <a name="create-userinstallstatesummary"></a><span data-ttu-id="23cd3-101">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="23cd3-101">Create userInstallStateSummary</span></span>

> <span data-ttu-id="23cd3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23cd3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23cd3-103">Criar um novo objeto [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="23cd3-103">Create a new [plannerBucket](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23cd3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23cd3-104">Prerequisites</span></span>
<span data-ttu-id="23cd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23cd3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23cd3-107">Permission type</span></span>|<span data-ttu-id="23cd3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23cd3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23cd3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23cd3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="23cd3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cd3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="23cd3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23cd3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cd3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cd3-112">Not supported.</span></span>|
|<span data-ttu-id="23cd3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23cd3-113">Application</span></span>|<span data-ttu-id="23cd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cd3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cd3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23cd3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="23cd3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23cd3-116">Request headers</span></span>
|<span data-ttu-id="23cd3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23cd3-117">Header</span></span>|<span data-ttu-id="23cd3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="23cd3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23cd3-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="23cd3-119">Authorization</span></span>|<span data-ttu-id="23cd3-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23cd3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23cd3-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23cd3-121">Accept</span></span>|<span data-ttu-id="23cd3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="23cd3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cd3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23cd3-123">Request body</span></span>
<span data-ttu-id="23cd3-124">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="23cd3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="23cd3-125">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="23cd3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="23cd3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23cd3-126">Property</span></span>|<span data-ttu-id="23cd3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cd3-127">Type</span></span>|<span data-ttu-id="23cd3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cd3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23cd3-129">id</span><span class="sxs-lookup"><span data-stu-id="23cd3-129">id</span></span>|<span data-ttu-id="23cd3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cd3-130">String</span></span>|<span data-ttu-id="23cd3-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23cd3-131">Key of the setting.</span></span>|
|<span data-ttu-id="23cd3-132">userName</span><span class="sxs-lookup"><span data-stu-id="23cd3-132">UserName</span></span>|<span data-ttu-id="23cd3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cd3-133">String</span></span>|<span data-ttu-id="23cd3-134">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="23cd3-134">User name.</span></span>|
|<span data-ttu-id="23cd3-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23cd3-135">installedDeviceCount</span></span>|<span data-ttu-id="23cd3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="23cd3-136">Int32</span></span>|<span data-ttu-id="23cd3-137">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="23cd3-137">Installed Device Count.</span></span>|
|<span data-ttu-id="23cd3-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23cd3-138">failedDeviceCount</span></span>|<span data-ttu-id="23cd3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="23cd3-139">Int32</span></span>|<span data-ttu-id="23cd3-140">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="23cd3-140">Failed Device Count.</span></span>|
|<span data-ttu-id="23cd3-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23cd3-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="23cd3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="23cd3-142">Int32</span></span>|<span data-ttu-id="23cd3-143">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="23cd3-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="23cd3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cd3-144">Response</span></span>
<span data-ttu-id="23cd3-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23cd3-145">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cd3-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23cd3-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="23cd3-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23cd3-147">Request</span></span>
<span data-ttu-id="23cd3-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23cd3-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="23cd3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cd3-149">Response</span></span>
<span data-ttu-id="23cd3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23cd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



