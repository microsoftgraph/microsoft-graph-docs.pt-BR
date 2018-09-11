# <a name="commit-action"></a><span data-ttu-id="8f310-101">ação de confirmação</span><span class="sxs-lookup"><span data-stu-id="8f310-101">commit action</span></span>

> <span data-ttu-id="8f310-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f310-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f310-103">Confirma um arquivo de um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f310-103">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f310-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f310-104">Prerequisites</span></span>
<span data-ttu-id="8f310-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8f310-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f310-107">Permission type</span></span>|<span data-ttu-id="8f310-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f310-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f310-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f310-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8f310-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f310-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f310-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f310-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f310-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f310-112">Not supported.</span></span>|
|<span data-ttu-id="8f310-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f310-113">Application</span></span>|<span data-ttu-id="8f310-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f310-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f310-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f310-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="8f310-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f310-116">Request headers</span></span>
|<span data-ttu-id="8f310-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f310-117">Header</span></span>|<span data-ttu-id="8f310-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8f310-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f310-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f310-119">Authorization</span></span>|<span data-ttu-id="8f310-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="8f310-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f310-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f310-121">Accept</span></span>|<span data-ttu-id="8f310-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8f310-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f310-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f310-123">Request body</span></span>
<span data-ttu-id="8f310-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8f310-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8f310-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8f310-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8f310-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f310-126">Property</span></span>|<span data-ttu-id="8f310-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f310-127">Type</span></span>|<span data-ttu-id="8f310-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f310-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f310-129">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="8f310-129">fileEncryptionInfo</span></span>|[<span data-ttu-id="8f310-130">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="8f310-130">fileEncryptionInfo</span></span>](../resources/intune_apps_fileencryptioninfo.md)|<span data-ttu-id="8f310-131">Chave de parâmetro das informações sobre criptografia de arquivo.</span><span class="sxs-lookup"><span data-stu-id="8f310-131">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="8f310-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f310-132">Response</span></span>
<span data-ttu-id="8f310-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f310-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f310-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f310-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f310-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f310-135">Request</span></span>
<span data-ttu-id="8f310-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f310-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="8f310-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f310-137">Response</span></span>
<span data-ttu-id="8f310-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








