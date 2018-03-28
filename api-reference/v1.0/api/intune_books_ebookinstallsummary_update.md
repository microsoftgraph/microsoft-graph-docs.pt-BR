# <a name="update-ebookinstallsummary"></a><span data-ttu-id="05839-101">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="05839-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="05839-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="05839-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05839-103">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05839-103">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05839-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05839-104">Prerequisites</span></span>
<span data-ttu-id="05839-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05839-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05839-107">Permission type</span></span>|<span data-ttu-id="05839-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05839-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05839-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05839-109">Delegated (work or school account)</span></span>|<span data-ttu-id="05839-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05839-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05839-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05839-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05839-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05839-112">Not supported.</span></span>|
|<span data-ttu-id="05839-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05839-113">Application</span></span>|<span data-ttu-id="05839-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05839-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05839-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05839-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="05839-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05839-116">Request headers</span></span>
|<span data-ttu-id="05839-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05839-117">Header</span></span>|<span data-ttu-id="05839-118">Valor</span><span class="sxs-lookup"><span data-stu-id="05839-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05839-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="05839-119">Authorization</span></span>|<span data-ttu-id="05839-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05839-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05839-121">Accept</span><span class="sxs-lookup"><span data-stu-id="05839-121">Accept</span></span>|<span data-ttu-id="05839-122">application/json</span><span class="sxs-lookup"><span data-stu-id="05839-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05839-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05839-123">Request body</span></span>
<span data-ttu-id="05839-124">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05839-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="05839-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05839-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="05839-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05839-126">Property</span></span>|<span data-ttu-id="05839-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="05839-127">Type</span></span>|<span data-ttu-id="05839-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="05839-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05839-129">id</span><span class="sxs-lookup"><span data-stu-id="05839-129">id</span></span>|<span data-ttu-id="05839-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05839-130">String</span></span>|<span data-ttu-id="05839-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05839-131">Key of the setting.</span></span>|
|<span data-ttu-id="05839-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05839-132">installedDeviceCount</span></span>|<span data-ttu-id="05839-133">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-133">Int32</span></span>|<span data-ttu-id="05839-134">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="05839-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="05839-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05839-135">failedDeviceCount</span></span>|<span data-ttu-id="05839-136">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-136">Int32</span></span>|<span data-ttu-id="05839-137">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="05839-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="05839-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05839-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="05839-139">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-139">Int32</span></span>|<span data-ttu-id="05839-140">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="05839-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="05839-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="05839-141">installedUserCount</span></span>|<span data-ttu-id="05839-142">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-142">Int32</span></span>|<span data-ttu-id="05839-143">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="05839-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="05839-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="05839-144">failedUserCount</span></span>|<span data-ttu-id="05839-145">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-145">Int32</span></span>|<span data-ttu-id="05839-146">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="05839-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="05839-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="05839-147">notInstalledUserCount</span></span>|<span data-ttu-id="05839-148">Int32</span><span class="sxs-lookup"><span data-stu-id="05839-148">Int32</span></span>|<span data-ttu-id="05839-149">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="05839-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="05839-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="05839-150">Response</span></span>
<span data-ttu-id="05839-151">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05839-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05839-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05839-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="05839-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05839-153">Request</span></span>
<span data-ttu-id="05839-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05839-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="05839-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="05839-155">Response</span></span>
<span data-ttu-id="05839-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05839-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```



