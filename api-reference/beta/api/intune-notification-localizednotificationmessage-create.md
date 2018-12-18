---
title: Criar localizedNotificationMessage
description: Criar um novo objeto localizedNotificationMessage.
author: tfitzmac
ms.openlocfilehash: 8070921493ec7430ee31376b0788d59013595184
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324357"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="65799-103">Criar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="65799-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="65799-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="65799-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65799-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65799-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65799-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="65799-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65799-107">Criar um novo objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="65799-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65799-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65799-108">Prerequisites</span></span>
<span data-ttu-id="65799-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65799-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65799-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65799-111">Permission type</span></span>|<span data-ttu-id="65799-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65799-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65799-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65799-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65799-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65799-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65799-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65799-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65799-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65799-116">Not supported.</span></span>|
|<span data-ttu-id="65799-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65799-117">Application</span></span>|<span data-ttu-id="65799-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65799-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65799-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65799-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="65799-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65799-120">Request headers</span></span>
|<span data-ttu-id="65799-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65799-121">Header</span></span>|<span data-ttu-id="65799-122">Valor</span><span class="sxs-lookup"><span data-stu-id="65799-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65799-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="65799-123">Authorization</span></span>|<span data-ttu-id="65799-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65799-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65799-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65799-125">Accept</span></span>|<span data-ttu-id="65799-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65799-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65799-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65799-127">Request body</span></span>
<span data-ttu-id="65799-128">No corpo da solicitação, forneça uma representação JSON do objeto localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="65799-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="65799-129">A tabela a seguir mostra as propriedades que são necessárias ao criar localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="65799-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="65799-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65799-130">Property</span></span>|<span data-ttu-id="65799-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="65799-131">Type</span></span>|<span data-ttu-id="65799-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="65799-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65799-133">id</span><span class="sxs-lookup"><span data-stu-id="65799-133">id</span></span>|<span data-ttu-id="65799-134">String</span><span class="sxs-lookup"><span data-stu-id="65799-134">String</span></span>|<span data-ttu-id="65799-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65799-135">Key of the entity.</span></span>|
|<span data-ttu-id="65799-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65799-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65799-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65799-137">DateTimeOffset</span></span>|<span data-ttu-id="65799-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="65799-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="65799-139">localidade</span><span class="sxs-lookup"><span data-stu-id="65799-139">locale</span></span>|<span data-ttu-id="65799-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65799-140">String</span></span>|<span data-ttu-id="65799-141">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="65799-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="65799-142">subject</span><span class="sxs-lookup"><span data-stu-id="65799-142">subject</span></span>|<span data-ttu-id="65799-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65799-143">String</span></span>|<span data-ttu-id="65799-144">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="65799-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="65799-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="65799-145">messageTemplate</span></span>|<span data-ttu-id="65799-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65799-146">String</span></span>|<span data-ttu-id="65799-147">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="65799-147">The Message Template content.</span></span>|
|<span data-ttu-id="65799-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="65799-148">isDefault</span></span>|<span data-ttu-id="65799-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="65799-149">Boolean</span></span>|<span data-ttu-id="65799-150">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="65799-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="65799-151">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="65799-151">This flag can only be set.</span></span> <span data-ttu-id="65799-152">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="65799-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="65799-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="65799-153">Response</span></span>
<span data-ttu-id="65799-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65799-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65799-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65799-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="65799-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65799-156">Request</span></span>
<span data-ttu-id="65799-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65799-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="65799-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="65799-158">Response</span></span>
<span data-ttu-id="65799-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65799-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





