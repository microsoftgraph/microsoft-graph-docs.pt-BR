---
title: Atualizar localizedNotificationMessage
description: Atualizar as propriedades de um objeto localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59b5aec3c8719b3531211baedfc1ed7592722f47
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262578"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="fce65-103">Atualizar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="fce65-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="fce65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fce65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fce65-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fce65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fce65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fce65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fce65-107">Atualizar as propriedades de um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fce65-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fce65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fce65-108">Prerequisites</span></span>
<span data-ttu-id="fce65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fce65-111">Permission type</span></span>|<span data-ttu-id="fce65-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fce65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fce65-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fce65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fce65-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce65-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fce65-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fce65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fce65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fce65-116">Not supported.</span></span>|
|<span data-ttu-id="fce65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fce65-117">Application</span></span>|<span data-ttu-id="fce65-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce65-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fce65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fce65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="fce65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fce65-120">Request headers</span></span>
|<span data-ttu-id="fce65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fce65-121">Header</span></span>|<span data-ttu-id="fce65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fce65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fce65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fce65-123">Authorization</span></span>|<span data-ttu-id="fce65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fce65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fce65-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fce65-125">Accept</span></span>|<span data-ttu-id="fce65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fce65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fce65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fce65-127">Request body</span></span>
<span data-ttu-id="fce65-128">No corpo da solicitação, forneça uma representação JSON do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fce65-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="fce65-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fce65-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="fce65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fce65-130">Property</span></span>|<span data-ttu-id="fce65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fce65-131">Type</span></span>|<span data-ttu-id="fce65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fce65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce65-133">id</span><span class="sxs-lookup"><span data-stu-id="fce65-133">id</span></span>|<span data-ttu-id="fce65-134">String</span><span class="sxs-lookup"><span data-stu-id="fce65-134">String</span></span>|<span data-ttu-id="fce65-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fce65-135">Key of the entity.</span></span>|
|<span data-ttu-id="fce65-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fce65-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fce65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fce65-137">DateTimeOffset</span></span>|<span data-ttu-id="fce65-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fce65-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fce65-139">localidade</span><span class="sxs-lookup"><span data-stu-id="fce65-139">locale</span></span>|<span data-ttu-id="fce65-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce65-140">String</span></span>|<span data-ttu-id="fce65-141">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="fce65-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="fce65-142">assunto</span><span class="sxs-lookup"><span data-stu-id="fce65-142">subject</span></span>|<span data-ttu-id="fce65-143">String</span><span class="sxs-lookup"><span data-stu-id="fce65-143">String</span></span>|<span data-ttu-id="fce65-144">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="fce65-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="fce65-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="fce65-145">messageTemplate</span></span>|<span data-ttu-id="fce65-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce65-146">String</span></span>|<span data-ttu-id="fce65-147">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="fce65-147">The Message Template content.</span></span>|
|<span data-ttu-id="fce65-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="fce65-148">isDefault</span></span>|<span data-ttu-id="fce65-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="fce65-149">Boolean</span></span>|<span data-ttu-id="fce65-150">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="fce65-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="fce65-151">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="fce65-151">This flag can only be set.</span></span> <span data-ttu-id="fce65-152">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="fce65-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="fce65-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce65-153">Response</span></span>
<span data-ttu-id="fce65-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fce65-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce65-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fce65-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fce65-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fce65-156">Request</span></span>
<span data-ttu-id="fce65-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fce65-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="fce65-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce65-158">Response</span></span>
<span data-ttu-id="fce65-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fce65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




