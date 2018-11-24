# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="aebee-101">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="aebee-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="aebee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aebee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aebee-103">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="aebee-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aebee-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aebee-104">Prerequisites</span></span>
<span data-ttu-id="aebee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aebee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aebee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aebee-107">Permission type</span></span>|<span data-ttu-id="aebee-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aebee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aebee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aebee-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="aebee-110">&nbsp;&nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="aebee-110">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="aebee-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebee-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aebee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aebee-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aebee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aebee-113">Not supported.</span></span>|
|<span data-ttu-id="aebee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aebee-114">Application</span></span>|<span data-ttu-id="aebee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aebee-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aebee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aebee-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="aebee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aebee-117">Request headers</span></span>
|<span data-ttu-id="aebee-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aebee-118">Header</span></span>|<span data-ttu-id="aebee-119">Valor</span><span class="sxs-lookup"><span data-stu-id="aebee-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aebee-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aebee-120">Authorization</span></span>|<span data-ttu-id="aebee-121">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aebee-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aebee-122">Accept</span><span class="sxs-lookup"><span data-stu-id="aebee-122">Accept</span></span>|<span data-ttu-id="aebee-123">application/json</span><span class="sxs-lookup"><span data-stu-id="aebee-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aebee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aebee-124">Request body</span></span>
<span data-ttu-id="aebee-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aebee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aebee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebee-126">Response</span></span>
<span data-ttu-id="aebee-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aebee-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="aebee-128">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="aebee-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="aebee-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebee-129">Response</span></span>

<span data-ttu-id="aebee-130">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="aebee-130">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aebee-131">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aebee-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



