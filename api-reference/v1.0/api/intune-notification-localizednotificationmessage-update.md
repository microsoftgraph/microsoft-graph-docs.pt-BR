---
title: Atualizar localizedNotificationMessage
description: Atualizar as propriedades de um objeto localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7699f0cab1459b3c876d6d78470c75c14c3bbdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055012"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="c8243-103">Atualizar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="c8243-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="c8243-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8243-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8243-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8243-106">Atualizar as propriedades de um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c8243-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8243-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8243-107">Prerequisites</span></span>
<span data-ttu-id="c8243-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8243-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8243-110">Permission type</span></span>|<span data-ttu-id="c8243-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8243-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8243-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8243-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8243-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8243-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8243-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8243-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8243-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8243-115">Not supported.</span></span>|
|<span data-ttu-id="c8243-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8243-116">Application</span></span>|<span data-ttu-id="c8243-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8243-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8243-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8243-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="c8243-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8243-119">Request headers</span></span>
|<span data-ttu-id="c8243-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8243-120">Header</span></span>|<span data-ttu-id="c8243-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8243-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8243-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8243-122">Authorization</span></span>|<span data-ttu-id="c8243-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8243-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8243-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8243-124">Accept</span></span>|<span data-ttu-id="c8243-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8243-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8243-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8243-126">Request body</span></span>
<span data-ttu-id="c8243-127">No corpo da solicitação, forneça uma representação JSON do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c8243-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="c8243-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c8243-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="c8243-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8243-129">Property</span></span>|<span data-ttu-id="c8243-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8243-130">Type</span></span>|<span data-ttu-id="c8243-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8243-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8243-132">id</span><span class="sxs-lookup"><span data-stu-id="c8243-132">id</span></span>|<span data-ttu-id="c8243-133">String</span><span class="sxs-lookup"><span data-stu-id="c8243-133">String</span></span>|<span data-ttu-id="c8243-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c8243-134">Key of the entity.</span></span>|
|<span data-ttu-id="c8243-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8243-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c8243-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8243-136">DateTimeOffset</span></span>|<span data-ttu-id="c8243-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c8243-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c8243-138">localidade</span><span class="sxs-lookup"><span data-stu-id="c8243-138">locale</span></span>|<span data-ttu-id="c8243-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8243-139">String</span></span>|<span data-ttu-id="c8243-140">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="c8243-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="c8243-141">assunto</span><span class="sxs-lookup"><span data-stu-id="c8243-141">subject</span></span>|<span data-ttu-id="c8243-142">String</span><span class="sxs-lookup"><span data-stu-id="c8243-142">String</span></span>|<span data-ttu-id="c8243-143">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c8243-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="c8243-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="c8243-144">messageTemplate</span></span>|<span data-ttu-id="c8243-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8243-145">String</span></span>|<span data-ttu-id="c8243-146">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c8243-146">The Message Template content.</span></span>|
|<span data-ttu-id="c8243-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="c8243-147">isDefault</span></span>|<span data-ttu-id="c8243-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8243-148">Boolean</span></span>|<span data-ttu-id="c8243-149">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="c8243-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="c8243-150">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="c8243-150">This flag can only be set.</span></span> <span data-ttu-id="c8243-151">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="c8243-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="c8243-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8243-152">Response</span></span>
<span data-ttu-id="c8243-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8243-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8243-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8243-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8243-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8243-155">Request</span></span>
<span data-ttu-id="c8243-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8243-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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

### <a name="response"></a><span data-ttu-id="c8243-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8243-157">Response</span></span>
<span data-ttu-id="c8243-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8243-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









