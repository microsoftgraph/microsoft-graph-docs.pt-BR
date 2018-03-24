# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="2e968-101">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="2e968-101">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="2e968-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2e968-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e968-103">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2e968-103">Update the properties of a [calendar](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e968-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e968-104">Prerequisites</span></span>
<span data-ttu-id="2e968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e968-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e968-107">Permission type</span></span>|<span data-ttu-id="2e968-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e968-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e968-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e968-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2e968-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e968-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e968-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e968-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e968-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e968-112">Not supported.</span></span>|
|<span data-ttu-id="2e968-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e968-113">Application</span></span>|<span data-ttu-id="2e968-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e968-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e968-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e968-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="2e968-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e968-116">Request headers</span></span>
|<span data-ttu-id="2e968-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e968-117">Header</span></span>|<span data-ttu-id="2e968-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2e968-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e968-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e968-119">Authorization</span></span>|<span data-ttu-id="2e968-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e968-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2e968-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e968-121">Accept</span></span>|<span data-ttu-id="2e968-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2e968-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e968-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e968-123">Request body</span></span>
<span data-ttu-id="2e968-124">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2e968-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="2e968-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2e968-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="2e968-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e968-126">Property</span></span>|<span data-ttu-id="2e968-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e968-127">Type</span></span>|<span data-ttu-id="2e968-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e968-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e968-129">id</span><span class="sxs-lookup"><span data-stu-id="2e968-129">id</span></span>|<span data-ttu-id="2e968-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e968-130">String</span></span>|<span data-ttu-id="2e968-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2e968-131">Key of the setting.</span></span>|
|<span data-ttu-id="2e968-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e968-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2e968-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e968-133">DateTimeOffset</span></span>|<span data-ttu-id="2e968-134">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2e968-134">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="2e968-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2e968-135">displayName</span></span>|<span data-ttu-id="2e968-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e968-136">String</span></span>|<span data-ttu-id="2e968-137">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="2e968-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="2e968-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="2e968-138">DefaultLocale</span></span>|<span data-ttu-id="2e968-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e968-139">String</span></span>|<span data-ttu-id="2e968-140">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="2e968-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="2e968-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="2e968-141">brandingOptions</span></span>|<span data-ttu-id="2e968-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e968-142">String</span></span>|<span data-ttu-id="2e968-143">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="2e968-143">The Message Template Branding Options.</span></span> <span data-ttu-id="2e968-144">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="2e968-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="2e968-145">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="2e968-145">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e968-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e968-146">Response</span></span>
<span data-ttu-id="2e968-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e968-147">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e968-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e968-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e968-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e968-149">Request</span></span>
<span data-ttu-id="2e968-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e968-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 195

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="2e968-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e968-151">Response</span></span>
<span data-ttu-id="2e968-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e968-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



