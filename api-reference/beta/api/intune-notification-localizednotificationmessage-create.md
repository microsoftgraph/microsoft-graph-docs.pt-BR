---
title: Criar localizedNotificationMessage
description: Criar um novo objeto localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ceb30b2dc6a154eb337684cb4eb5816453846886
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064910"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="50244-103">Criar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="50244-103">Create localizedNotificationMessage</span></span>

<span data-ttu-id="50244-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50244-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50244-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50244-107">Criar um novo objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="50244-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50244-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50244-108">Prerequisites</span></span>
<span data-ttu-id="50244-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50244-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50244-111">Permission type</span></span>|<span data-ttu-id="50244-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50244-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50244-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50244-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50244-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50244-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50244-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50244-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50244-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50244-116">Not supported.</span></span>|
|<span data-ttu-id="50244-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50244-117">Application</span></span>|<span data-ttu-id="50244-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50244-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50244-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50244-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="50244-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50244-120">Request headers</span></span>
|<span data-ttu-id="50244-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50244-121">Header</span></span>|<span data-ttu-id="50244-122">Valor</span><span class="sxs-lookup"><span data-stu-id="50244-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50244-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="50244-123">Authorization</span></span>|<span data-ttu-id="50244-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50244-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50244-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50244-125">Accept</span></span>|<span data-ttu-id="50244-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50244-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50244-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50244-127">Request body</span></span>
<span data-ttu-id="50244-128">No corpo da solicitação, forneça uma representação JSON do objeto localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="50244-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="50244-129">A tabela a seguir mostra as propriedades que são necessárias ao criar localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="50244-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="50244-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50244-130">Property</span></span>|<span data-ttu-id="50244-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="50244-131">Type</span></span>|<span data-ttu-id="50244-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="50244-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50244-133">id</span><span class="sxs-lookup"><span data-stu-id="50244-133">id</span></span>|<span data-ttu-id="50244-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50244-134">String</span></span>|<span data-ttu-id="50244-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50244-135">Key of the entity.</span></span>|
|<span data-ttu-id="50244-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50244-136">lastModifiedDateTime</span></span>|<span data-ttu-id="50244-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50244-137">DateTimeOffset</span></span>|<span data-ttu-id="50244-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="50244-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="50244-139">localidade</span><span class="sxs-lookup"><span data-stu-id="50244-139">locale</span></span>|<span data-ttu-id="50244-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50244-140">String</span></span>|<span data-ttu-id="50244-141">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="50244-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="50244-142">subject</span><span class="sxs-lookup"><span data-stu-id="50244-142">subject</span></span>|<span data-ttu-id="50244-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50244-143">String</span></span>|<span data-ttu-id="50244-144">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50244-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="50244-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="50244-145">messageTemplate</span></span>|<span data-ttu-id="50244-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50244-146">String</span></span>|<span data-ttu-id="50244-147">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50244-147">The Message Template content.</span></span>|
|<span data-ttu-id="50244-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="50244-148">isDefault</span></span>|<span data-ttu-id="50244-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="50244-149">Boolean</span></span>|<span data-ttu-id="50244-150">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="50244-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="50244-151">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="50244-151">This flag can only be set.</span></span> <span data-ttu-id="50244-152">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="50244-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="50244-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="50244-153">Response</span></span>
<span data-ttu-id="50244-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50244-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50244-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50244-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="50244-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50244-156">Request</span></span>
<span data-ttu-id="50244-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50244-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="50244-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="50244-158">Response</span></span>
<span data-ttu-id="50244-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50244-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






