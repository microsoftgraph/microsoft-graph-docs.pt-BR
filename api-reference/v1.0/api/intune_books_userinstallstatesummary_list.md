# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="c7573-101">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c7573-101">List userInstallStateSummaries</span></span>

> <span data-ttu-id="c7573-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7573-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7573-103">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c7573-103">List properties and relationships of the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7573-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7573-104">Prerequisites</span></span>
<span data-ttu-id="c7573-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7573-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7573-107">Permission type</span></span>|<span data-ttu-id="c7573-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7573-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7573-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7573-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c7573-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7573-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c7573-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7573-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7573-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7573-112">Not supported.</span></span>|
|<span data-ttu-id="c7573-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7573-113">Application</span></span>|<span data-ttu-id="c7573-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7573-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7573-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7573-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c7573-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7573-116">Request headers</span></span>
|<span data-ttu-id="c7573-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7573-117">Header</span></span>|<span data-ttu-id="c7573-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c7573-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7573-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7573-119">Authorization</span></span>|<span data-ttu-id="c7573-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="c7573-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7573-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7573-121">Accept</span></span>|<span data-ttu-id="c7573-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c7573-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7573-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7573-123">Request body</span></span>
<span data-ttu-id="c7573-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7573-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7573-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7573-125">Response</span></span>
<span data-ttu-id="c7573-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7573-126">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7573-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7573-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7573-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7573-128">Request</span></span>
<span data-ttu-id="c7573-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7573-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="c7573-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7573-130">Response</span></span>
<span data-ttu-id="c7573-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7573-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```








