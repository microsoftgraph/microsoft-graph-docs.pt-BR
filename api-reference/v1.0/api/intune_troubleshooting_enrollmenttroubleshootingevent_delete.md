# <a name="delete-enrollmenttroubleshootingevent"></a><span data-ttu-id="8f940-101">Excluir enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8f940-101">Delete enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="8f940-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f940-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f940-103">Exclui [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8f940-103">Deletes a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f940-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f940-104">Prerequisites</span></span>
<span data-ttu-id="8f940-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8f940-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f940-107">Permission type</span></span>|<span data-ttu-id="8f940-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f940-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f940-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f940-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8f940-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f940-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8f940-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f940-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f940-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f940-112">Not supported.</span></span>|
|<span data-ttu-id="8f940-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f940-113">Application</span></span>|<span data-ttu-id="8f940-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f940-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f940-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f940-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="8f940-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f940-116">Request headers</span></span>
|<span data-ttu-id="8f940-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f940-117">Header</span></span>|<span data-ttu-id="8f940-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8f940-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f940-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f940-119">Authorization</span></span>|<span data-ttu-id="8f940-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f940-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f940-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8f940-121">Accept</span></span>|<span data-ttu-id="8f940-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8f940-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f940-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f940-123">Request body</span></span>
<span data-ttu-id="8f940-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f940-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f940-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f940-125">Response</span></span>
<span data-ttu-id="8f940-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f940-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f940-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f940-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f940-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f940-128">Request</span></span>
<span data-ttu-id="8f940-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f940-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="8f940-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f940-130">Response</span></span>
<span data-ttu-id="8f940-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f940-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



