# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="19c2b-101">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="19c2b-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="19c2b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19c2b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19c2b-103">Criar um novo objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="19c2b-103">Create a new [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19c2b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19c2b-104">Prerequisites</span></span>
<span data-ttu-id="19c2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19c2b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19c2b-107">Permission type</span></span>|<span data-ttu-id="19c2b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19c2b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19c2b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19c2b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="19c2b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c2b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="19c2b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19c2b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19c2b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19c2b-112">Not supported.</span></span>|
|<span data-ttu-id="19c2b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19c2b-113">Application</span></span>|<span data-ttu-id="19c2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19c2b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19c2b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19c2b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="19c2b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19c2b-116">Request headers</span></span>
|<span data-ttu-id="19c2b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19c2b-117">Header</span></span>|<span data-ttu-id="19c2b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="19c2b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19c2b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="19c2b-119">Authorization</span></span>|<span data-ttu-id="19c2b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19c2b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19c2b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19c2b-121">Accept</span></span>|<span data-ttu-id="19c2b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="19c2b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19c2b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19c2b-123">Request body</span></span>
<span data-ttu-id="19c2b-124">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="19c2b-124">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="19c2b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="19c2b-125">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="19c2b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19c2b-126">Property</span></span>|<span data-ttu-id="19c2b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="19c2b-127">Type</span></span>|<span data-ttu-id="19c2b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="19c2b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c2b-129">id</span><span class="sxs-lookup"><span data-stu-id="19c2b-129">id</span></span>|<span data-ttu-id="19c2b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c2b-130">String</span></span>|<span data-ttu-id="19c2b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19c2b-131">Key of the entity.</span></span>|
|<span data-ttu-id="19c2b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19c2b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="19c2b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c2b-133">DateTimeOffset</span></span>|<span data-ttu-id="19c2b-134">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="19c2b-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="19c2b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="19c2b-135">displayName</span></span>|<span data-ttu-id="19c2b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c2b-136">String</span></span>|<span data-ttu-id="19c2b-137">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="19c2b-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="19c2b-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="19c2b-138">defaultLocale</span></span>|<span data-ttu-id="19c2b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c2b-139">String</span></span>|<span data-ttu-id="19c2b-140">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="19c2b-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="19c2b-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="19c2b-141">brandingOptions</span></span>|[<span data-ttu-id="19c2b-142">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="19c2b-142">notificationTemplateBrandingOptions</span></span>](../resources/intune_notification_notificationtemplatebrandingoptions.md)|<span data-ttu-id="19c2b-143">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="19c2b-143">The Message Template Branding Options.</span></span> <span data-ttu-id="19c2b-144">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="19c2b-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="19c2b-145">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="19c2b-145">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="19c2b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c2b-146">Response</span></span>
<span data-ttu-id="19c2b-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19c2b-147">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19c2b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19c2b-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="19c2b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19c2b-149">Request</span></span>
<span data-ttu-id="19c2b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19c2b-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="19c2b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c2b-151">Response</span></span>
<span data-ttu-id="19c2b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19c2b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```



