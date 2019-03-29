---
title: Criar localizedNotificationMessage
description: Criar um novo objeto localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 919e7feea0643d4e62e715d31bd7a8f5d82ce3de
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974654"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="22052-103">Criar localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="22052-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="22052-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22052-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22052-105">Criar um novo objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="22052-105">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22052-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22052-106">Prerequisites</span></span>
<span data-ttu-id="22052-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22052-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22052-109">Permission type</span></span>|<span data-ttu-id="22052-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22052-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22052-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22052-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22052-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22052-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22052-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22052-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22052-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22052-114">Not supported.</span></span>|
|<span data-ttu-id="22052-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22052-115">Application</span></span>|<span data-ttu-id="22052-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22052-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22052-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22052-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="22052-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22052-118">Request headers</span></span>
|<span data-ttu-id="22052-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22052-119">Header</span></span>|<span data-ttu-id="22052-120">Valor</span><span class="sxs-lookup"><span data-stu-id="22052-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22052-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22052-121">Authorization</span></span>|<span data-ttu-id="22052-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22052-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22052-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22052-123">Accept</span></span>|<span data-ttu-id="22052-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22052-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22052-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22052-125">Request body</span></span>
<span data-ttu-id="22052-126">No corpo da solicitação, forneça uma representação JSON do objeto localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="22052-126">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="22052-127">A tabela a seguir mostra as propriedades que são necessárias ao criar localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="22052-127">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="22052-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22052-128">Property</span></span>|<span data-ttu-id="22052-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="22052-129">Type</span></span>|<span data-ttu-id="22052-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="22052-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22052-131">id</span><span class="sxs-lookup"><span data-stu-id="22052-131">id</span></span>|<span data-ttu-id="22052-132">String</span><span class="sxs-lookup"><span data-stu-id="22052-132">String</span></span>|<span data-ttu-id="22052-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22052-133">Key of the entity.</span></span>|
|<span data-ttu-id="22052-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22052-134">lastModifiedDateTime</span></span>|<span data-ttu-id="22052-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22052-135">DateTimeOffset</span></span>|<span data-ttu-id="22052-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22052-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="22052-137">localidade</span><span class="sxs-lookup"><span data-stu-id="22052-137">locale</span></span>|<span data-ttu-id="22052-138">String</span><span class="sxs-lookup"><span data-stu-id="22052-138">String</span></span>|<span data-ttu-id="22052-139">A localidade para a qual esta mensagem se destina.</span><span class="sxs-lookup"><span data-stu-id="22052-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="22052-140">Assunto</span><span class="sxs-lookup"><span data-stu-id="22052-140">subject</span></span>|<span data-ttu-id="22052-141">String</span><span class="sxs-lookup"><span data-stu-id="22052-141">String</span></span>|<span data-ttu-id="22052-142">O assunto do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="22052-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="22052-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="22052-143">messageTemplate</span></span>|<span data-ttu-id="22052-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22052-144">String</span></span>|<span data-ttu-id="22052-145">O conteúdo do modelo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="22052-145">The Message Template content.</span></span>|
|<span data-ttu-id="22052-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="22052-146">isDefault</span></span>|<span data-ttu-id="22052-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="22052-147">Boolean</span></span>|<span data-ttu-id="22052-148">Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma.</span><span class="sxs-lookup"><span data-stu-id="22052-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="22052-149">Esse sinalizador só pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="22052-149">This flag can only be set.</span></span> <span data-ttu-id="22052-150">Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.</span><span class="sxs-lookup"><span data-stu-id="22052-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="22052-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="22052-151">Response</span></span>
<span data-ttu-id="22052-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22052-152">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22052-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22052-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="22052-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22052-154">Request</span></span>
<span data-ttu-id="22052-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22052-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="22052-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="22052-156">Response</span></span>
<span data-ttu-id="22052-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22052-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



