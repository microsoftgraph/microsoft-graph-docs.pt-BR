# <a name="delete-devicecategory"></a><span data-ttu-id="27f12-101">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="27f12-101">Delete deviceCategory</span></span>

> <span data-ttu-id="27f12-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="27f12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27f12-103">Exclui [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="27f12-103">Deletes a [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27f12-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27f12-104">Prerequisites</span></span>
<span data-ttu-id="27f12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27f12-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27f12-107">Permission type</span></span>|<span data-ttu-id="27f12-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27f12-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27f12-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27f12-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27f12-110">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="27f12-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="27f12-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f12-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27f12-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27f12-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27f12-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f12-113">Not supported.</span></span>|
|<span data-ttu-id="27f12-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27f12-114">Application</span></span>|<span data-ttu-id="27f12-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f12-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27f12-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27f12-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="27f12-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27f12-117">Request headers</span></span>
|<span data-ttu-id="27f12-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27f12-118">Header</span></span>|<span data-ttu-id="27f12-119">Valor</span><span class="sxs-lookup"><span data-stu-id="27f12-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27f12-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="27f12-120">Authorization</span></span>|<span data-ttu-id="27f12-121">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f12-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27f12-122">Accept</span><span class="sxs-lookup"><span data-stu-id="27f12-122">Accept</span></span>|<span data-ttu-id="27f12-123">application/json</span><span class="sxs-lookup"><span data-stu-id="27f12-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27f12-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27f12-124">Request body</span></span>
<span data-ttu-id="27f12-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27f12-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27f12-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f12-126">Response</span></span>
<span data-ttu-id="27f12-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27f12-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27f12-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27f12-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="27f12-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27f12-129">Request</span></span>
<span data-ttu-id="27f12-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f12-130">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="27f12-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f12-131">Response</span></span>
<span data-ttu-id="27f12-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27f12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



