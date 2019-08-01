---
title: Atualizar localizedNotificationMessage
description: Atualizar as propriedades de um objeto localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c7b031ec6ff7007e459715d01a932970a5ceaa8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974777"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="784e3-103">Atualizar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="784e3-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="784e3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="784e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="784e3-105">Atualizar as propriedades de um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="784e3-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="784e3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="784e3-106">Prerequisites</span></span>
<span data-ttu-id="784e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="784e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="784e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="784e3-109">Permission type</span></span>|<span data-ttu-id="784e3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="784e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="784e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="784e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="784e3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="784e3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="784e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="784e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="784e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784e3-114">Not supported.</span></span>|
|<span data-ttu-id="784e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="784e3-115">Application</span></span>|<span data-ttu-id="784e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="784e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="784e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="784e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="784e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="784e3-118">Request headers</span></span>
|<span data-ttu-id="784e3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="784e3-119">Header</span></span>|<span data-ttu-id="784e3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="784e3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="784e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="784e3-121">Authorization</span></span>|<span data-ttu-id="784e3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="784e3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="784e3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="784e3-123">Accept</span></span>|<span data-ttu-id="784e3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="784e3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="784e3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="784e3-125">Request body</span></span>
<span data-ttu-id="784e3-126">No corpo da solicitação, forneça uma representação JSON do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="784e3-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="784e3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="784e3-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="784e3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="784e3-128">Property</span></span>|<span data-ttu-id="784e3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="784e3-129">Type</span></span>|<span data-ttu-id="784e3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="784e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="784e3-131">id</span><span class="sxs-lookup"><span data-stu-id="784e3-131">id</span></span>|<span data-ttu-id="784e3-132">String</span><span class="sxs-lookup"><span data-stu-id="784e3-132">String</span></span>|<span data-ttu-id="784e3-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="784e3-133">Key of the entity.</span></span>|
|<span data-ttu-id="784e3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="784e3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="784e3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="784e3-135">DateTimeOffset</span></span>|<span data-ttu-id="784e3-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="784e3-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="784e3-137">localidade</span><span class="sxs-lookup"><span data-stu-id="784e3-137">locale</span></span>|<span data-ttu-id="784e3-138">String</span><span class="sxs-lookup"><span data-stu-id="784e3-138">String</span></span>|<span data-ttu-id="784e3-139">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="784e3-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="784e3-140">subject</span><span class="sxs-lookup"><span data-stu-id="784e3-140">subject</span></span>|<span data-ttu-id="784e3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="784e3-141">String</span></span>|<span data-ttu-id="784e3-142">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="784e3-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="784e3-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="784e3-143">messageTemplate</span></span>|<span data-ttu-id="784e3-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="784e3-144">String</span></span>|<span data-ttu-id="784e3-145">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="784e3-145">The Message Template content.</span></span>|
|<span data-ttu-id="784e3-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="784e3-146">isDefault</span></span>|<span data-ttu-id="784e3-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="784e3-147">Boolean</span></span>|<span data-ttu-id="784e3-148">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="784e3-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="784e3-149">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="784e3-149">This flag can only be set.</span></span> <span data-ttu-id="784e3-150">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="784e3-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="784e3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="784e3-151">Response</span></span>
<span data-ttu-id="784e3-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="784e3-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="784e3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="784e3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="784e3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="784e3-154">Request</span></span>
<span data-ttu-id="784e3-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="784e3-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="784e3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="784e3-156">Response</span></span>
<span data-ttu-id="784e3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="784e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



