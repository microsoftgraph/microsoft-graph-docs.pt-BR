# <a name="list-managedebooks"></a><span data-ttu-id="b9536-101">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="b9536-101">List managedEBooks</span></span>

> <span data-ttu-id="b9536-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9536-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9536-103">Listar propriedades e relações dos objetos [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b9536-103">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9536-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9536-104">Prerequisites</span></span>
<span data-ttu-id="b9536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9536-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9536-107">Permission type</span></span>|<span data-ttu-id="b9536-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9536-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9536-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9536-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b9536-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9536-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b9536-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9536-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9536-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9536-112">Not supported.</span></span>|
|<span data-ttu-id="b9536-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9536-113">Application</span></span>|<span data-ttu-id="b9536-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9536-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9536-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9536-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="b9536-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9536-116">Request headers</span></span>
|<span data-ttu-id="b9536-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9536-117">Header</span></span>|<span data-ttu-id="b9536-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b9536-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9536-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9536-119">Authorization</span></span>|<span data-ttu-id="b9536-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9536-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b9536-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9536-121">Accept</span></span>|<span data-ttu-id="b9536-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b9536-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9536-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9536-123">Request body</span></span>
<span data-ttu-id="b9536-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9536-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9536-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9536-125">Response</span></span>
<span data-ttu-id="b9536-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune_books_managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9536-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_books_managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9536-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9536-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9536-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9536-128">Request</span></span>
<span data-ttu-id="b9536-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9536-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="b9536-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9536-130">Response</span></span>
<span data-ttu-id="b9536-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```



