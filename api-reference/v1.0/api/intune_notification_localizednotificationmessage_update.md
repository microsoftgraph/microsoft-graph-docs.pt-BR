# <a name="update-localizednotificationmessage"></a><span data-ttu-id="39e8d-101">Atualizar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="39e8d-101">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="39e8d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="39e8d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39e8d-103">Atualizar as propriedades de um objeto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="39e8d-103">Update the properties of a [calendar](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39e8d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39e8d-104">Prerequisites</span></span>
<span data-ttu-id="39e8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39e8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39e8d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39e8d-107">Permission type</span></span>|<span data-ttu-id="39e8d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39e8d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39e8d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39e8d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="39e8d-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39e8d-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="39e8d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39e8d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39e8d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39e8d-112">Not supported.</span></span>|
|<span data-ttu-id="39e8d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39e8d-113">Application</span></span>|<span data-ttu-id="39e8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39e8d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39e8d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39e8d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="39e8d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39e8d-116">Request headers</span></span>
|<span data-ttu-id="39e8d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39e8d-117">Header</span></span>|<span data-ttu-id="39e8d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="39e8d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39e8d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="39e8d-119">Authorization</span></span>|<span data-ttu-id="39e8d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39e8d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="39e8d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39e8d-121">Accept</span></span>|<span data-ttu-id="39e8d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="39e8d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39e8d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39e8d-123">Request body</span></span>
<span data-ttu-id="39e8d-124">No corpo da solicitação, forneça uma representação JSON do objeto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="39e8d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="39e8d-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="39e8d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="39e8d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39e8d-126">Property</span></span>|<span data-ttu-id="39e8d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="39e8d-127">Type</span></span>|<span data-ttu-id="39e8d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="39e8d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39e8d-129">id</span><span class="sxs-lookup"><span data-stu-id="39e8d-129">id</span></span>|<span data-ttu-id="39e8d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e8d-130">String</span></span>|<span data-ttu-id="39e8d-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39e8d-131">Key of the setting.</span></span>|
|<span data-ttu-id="39e8d-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39e8d-132">lastModifiedDateTime</span></span>|<span data-ttu-id="39e8d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39e8d-133">DateTimeOffset</span></span>|<span data-ttu-id="39e8d-134">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="39e8d-134">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="39e8d-135">localidade</span><span class="sxs-lookup"><span data-stu-id="39e8d-135">locale</span></span>|<span data-ttu-id="39e8d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e8d-136">String</span></span>|<span data-ttu-id="39e8d-137">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="39e8d-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="39e8d-138">subject</span><span class="sxs-lookup"><span data-stu-id="39e8d-138">subject</span></span>|<span data-ttu-id="39e8d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e8d-139">String</span></span>|<span data-ttu-id="39e8d-140">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="39e8d-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="39e8d-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="39e8d-141">messageTemplate</span></span>|<span data-ttu-id="39e8d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e8d-142">String</span></span>|<span data-ttu-id="39e8d-143">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="39e8d-143">The Message Template content.</span></span>|
|<span data-ttu-id="39e8d-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="39e8d-144">isDefault</span></span>|<span data-ttu-id="39e8d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="39e8d-145">Boolean</span></span>|<span data-ttu-id="39e8d-146">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="39e8d-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="39e8d-147">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="39e8d-147">This flag can only be set.</span></span> <span data-ttu-id="39e8d-148">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="39e8d-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="39e8d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="39e8d-149">Response</span></span>
<span data-ttu-id="39e8d-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39e8d-150">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39e8d-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39e8d-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="39e8d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39e8d-152">Request</span></span>
<span data-ttu-id="39e8d-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39e8d-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="39e8d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="39e8d-154">Response</span></span>
<span data-ttu-id="39e8d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39e8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```



