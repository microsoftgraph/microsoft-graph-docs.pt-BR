---
title: Atualizar localizedNotificationMessage
description: Atualizar as propriedades de um objeto localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fdd3066f0f5b9228008143409d63ceeeecf5c21
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727763"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="22a6e-103">Atualizar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="22a6e-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="22a6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a6e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22a6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22a6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a6e-107">Atualizar as propriedades de um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="22a6e-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22a6e-108">Prerequisites</span></span>
<span data-ttu-id="22a6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a6e-111">Permission type</span></span>|<span data-ttu-id="22a6e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22a6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a6e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a6e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22a6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a6e-116">Not supported.</span></span>|
|<span data-ttu-id="22a6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a6e-117">Application</span></span>|<span data-ttu-id="22a6e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a6e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="22a6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a6e-120">Request headers</span></span>
|<span data-ttu-id="22a6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22a6e-121">Header</span></span>|<span data-ttu-id="22a6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22a6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a6e-123">Authorization</span></span>|<span data-ttu-id="22a6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a6e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22a6e-125">Accept</span></span>|<span data-ttu-id="22a6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a6e-127">Request body</span></span>
<span data-ttu-id="22a6e-128">No corpo da solicitação, forneça uma representação JSON do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="22a6e-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="22a6e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="22a6e-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="22a6e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a6e-130">Property</span></span>|<span data-ttu-id="22a6e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a6e-131">Type</span></span>|<span data-ttu-id="22a6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a6e-133">id</span><span class="sxs-lookup"><span data-stu-id="22a6e-133">id</span></span>|<span data-ttu-id="22a6e-134">String</span><span class="sxs-lookup"><span data-stu-id="22a6e-134">String</span></span>|<span data-ttu-id="22a6e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22a6e-135">Key of the entity.</span></span>|
|<span data-ttu-id="22a6e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22a6e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="22a6e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a6e-137">DateTimeOffset</span></span>|<span data-ttu-id="22a6e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22a6e-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="22a6e-139">localidade</span><span class="sxs-lookup"><span data-stu-id="22a6e-139">locale</span></span>|<span data-ttu-id="22a6e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22a6e-140">String</span></span>|<span data-ttu-id="22a6e-141">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="22a6e-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="22a6e-142">assunto</span><span class="sxs-lookup"><span data-stu-id="22a6e-142">subject</span></span>|<span data-ttu-id="22a6e-143">String</span><span class="sxs-lookup"><span data-stu-id="22a6e-143">String</span></span>|<span data-ttu-id="22a6e-144">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="22a6e-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="22a6e-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="22a6e-145">messageTemplate</span></span>|<span data-ttu-id="22a6e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22a6e-146">String</span></span>|<span data-ttu-id="22a6e-147">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="22a6e-147">The Message Template content.</span></span>|
|<span data-ttu-id="22a6e-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="22a6e-148">isDefault</span></span>|<span data-ttu-id="22a6e-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="22a6e-149">Boolean</span></span>|<span data-ttu-id="22a6e-150">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="22a6e-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="22a6e-151">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="22a6e-151">This flag can only be set.</span></span> <span data-ttu-id="22a6e-152">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="22a6e-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="22a6e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a6e-153">Response</span></span>
<span data-ttu-id="22a6e-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a6e-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a6e-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a6e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a6e-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a6e-156">Request</span></span>
<span data-ttu-id="22a6e-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a6e-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22a6e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a6e-158">Response</span></span>
<span data-ttu-id="22a6e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22a6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





