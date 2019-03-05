---
title: Criar localizedNotificationMessage
description: Criar um novo objeto localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af7024f2218bb56f9f6cbf6a633c6513e50fdb9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147695"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="9d8d6-103">Criar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9d8d6-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="9d8d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d8d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d8d6-106">Criar um novo objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="9d8d6-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d8d6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d8d6-107">Prerequisites</span></span>
<span data-ttu-id="9d8d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d8d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9d8d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d8d6-110">Permission type</span></span>|<span data-ttu-id="9d8d6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d8d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d8d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d8d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d8d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9d8d6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d8d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d8d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-115">Not supported.</span></span>|
|<span data-ttu-id="9d8d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d8d6-116">Application</span></span>|<span data-ttu-id="9d8d6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d8d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d8d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="9d8d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8d6-119">Request headers</span></span>
|<span data-ttu-id="9d8d6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d8d6-120">Header</span></span>|<span data-ttu-id="9d8d6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9d8d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d8d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d8d6-122">Authorization</span></span>|<span data-ttu-id="9d8d6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d8d6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d8d6-124">Accept</span></span>|<span data-ttu-id="9d8d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d8d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d8d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8d6-126">Request body</span></span>
<span data-ttu-id="9d8d6-127">No corpo da solicitação, forneça uma representação JSON do objeto localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="9d8d6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="9d8d6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d8d6-129">Property</span></span>|<span data-ttu-id="9d8d6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d8d6-130">Type</span></span>|<span data-ttu-id="9d8d6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d8d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8d6-132">id</span><span class="sxs-lookup"><span data-stu-id="9d8d6-132">id</span></span>|<span data-ttu-id="9d8d6-133">String</span><span class="sxs-lookup"><span data-stu-id="9d8d6-133">String</span></span>|<span data-ttu-id="9d8d6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-134">Key of the entity.</span></span>|
|<span data-ttu-id="9d8d6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d8d6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9d8d6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d8d6-136">DateTimeOffset</span></span>|<span data-ttu-id="9d8d6-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9d8d6-138">localidade</span><span class="sxs-lookup"><span data-stu-id="9d8d6-138">locale</span></span>|<span data-ttu-id="9d8d6-139">String</span><span class="sxs-lookup"><span data-stu-id="9d8d6-139">String</span></span>|<span data-ttu-id="9d8d6-140">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="9d8d6-141">subject</span><span class="sxs-lookup"><span data-stu-id="9d8d6-141">subject</span></span>|<span data-ttu-id="9d8d6-142">String</span><span class="sxs-lookup"><span data-stu-id="9d8d6-142">String</span></span>|<span data-ttu-id="9d8d6-143">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="9d8d6-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="9d8d6-144">messageTemplate</span></span>|<span data-ttu-id="9d8d6-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d8d6-145">String</span></span>|<span data-ttu-id="9d8d6-146">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-146">The Message Template content.</span></span>|
|<span data-ttu-id="9d8d6-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="9d8d6-147">isDefault</span></span>|<span data-ttu-id="9d8d6-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d8d6-148">Boolean</span></span>|<span data-ttu-id="9d8d6-149">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="9d8d6-150">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-150">This flag can only be set.</span></span> <span data-ttu-id="9d8d6-151">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="9d8d6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d8d6-152">Response</span></span>
<span data-ttu-id="9d8d6-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d8d6-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d8d6-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d8d6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8d6-155">Request</span></span>
<span data-ttu-id="9d8d6-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d8d6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d8d6-157">Response</span></span>
<span data-ttu-id="9d8d6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d8d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




