# <a name="delete-androidmanagedappregistration"></a><span data-ttu-id="57898-101">Excluir androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57898-101">Delete androidManagedAppRegistration</span></span>

> <span data-ttu-id="57898-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57898-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57898-103">Exclui [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="57898-103">Deletes a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57898-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57898-104">Prerequisites</span></span>
<span data-ttu-id="57898-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57898-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57898-107">Permission type</span></span>|<span data-ttu-id="57898-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57898-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57898-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57898-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57898-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57898-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57898-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57898-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57898-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57898-112">Not supported.</span></span>|
|<span data-ttu-id="57898-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57898-113">Application</span></span>|<span data-ttu-id="57898-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57898-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57898-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57898-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="57898-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57898-116">Request headers</span></span>
|<span data-ttu-id="57898-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57898-117">Header</span></span>|<span data-ttu-id="57898-118">Valor</span><span class="sxs-lookup"><span data-stu-id="57898-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57898-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="57898-119">Authorization</span></span>|<span data-ttu-id="57898-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57898-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57898-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57898-121">Accept</span></span>|<span data-ttu-id="57898-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57898-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57898-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57898-123">Request body</span></span>
<span data-ttu-id="57898-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57898-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57898-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="57898-125">Response</span></span>
<span data-ttu-id="57898-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57898-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57898-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57898-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="57898-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57898-128">Request</span></span>
<span data-ttu-id="57898-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57898-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="57898-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="57898-130">Response</span></span>
<span data-ttu-id="57898-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57898-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



