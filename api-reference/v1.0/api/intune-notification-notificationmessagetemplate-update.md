---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23fc5364a39969ae137796cfc461e8cf19ae26d0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751479"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="6b57e-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="6b57e-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="6b57e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b57e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b57e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b57e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b57e-106">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="6b57e-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b57e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b57e-107">Prerequisites</span></span>
<span data-ttu-id="6b57e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b57e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b57e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b57e-110">Permission type</span></span>|<span data-ttu-id="6b57e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b57e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b57e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b57e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b57e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b57e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6b57e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b57e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b57e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b57e-115">Not supported.</span></span>|
|<span data-ttu-id="6b57e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b57e-116">Application</span></span>|<span data-ttu-id="6b57e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b57e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b57e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b57e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="6b57e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b57e-119">Request headers</span></span>
|<span data-ttu-id="6b57e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b57e-120">Header</span></span>|<span data-ttu-id="6b57e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b57e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b57e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b57e-122">Authorization</span></span>|<span data-ttu-id="6b57e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b57e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b57e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b57e-124">Accept</span></span>|<span data-ttu-id="6b57e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b57e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b57e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b57e-126">Request body</span></span>
<span data-ttu-id="6b57e-127">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="6b57e-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="6b57e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="6b57e-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="6b57e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b57e-129">Property</span></span>|<span data-ttu-id="6b57e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b57e-130">Type</span></span>|<span data-ttu-id="6b57e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b57e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b57e-132">id</span><span class="sxs-lookup"><span data-stu-id="6b57e-132">id</span></span>|<span data-ttu-id="6b57e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b57e-133">String</span></span>|<span data-ttu-id="6b57e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b57e-134">Key of the entity.</span></span>|
|<span data-ttu-id="6b57e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b57e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6b57e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b57e-136">DateTimeOffset</span></span>|<span data-ttu-id="6b57e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b57e-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6b57e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6b57e-138">displayName</span></span>|<span data-ttu-id="6b57e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b57e-139">String</span></span>|<span data-ttu-id="6b57e-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="6b57e-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="6b57e-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="6b57e-141">defaultLocale</span></span>|<span data-ttu-id="6b57e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b57e-142">String</span></span>|<span data-ttu-id="6b57e-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="6b57e-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="6b57e-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="6b57e-144">brandingOptions</span></span>|[<span data-ttu-id="6b57e-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="6b57e-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="6b57e-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="6b57e-146">The Message Template Branding Options.</span></span> <span data-ttu-id="6b57e-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="6b57e-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="6b57e-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="6b57e-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="6b57e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b57e-149">Response</span></span>
<span data-ttu-id="6b57e-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b57e-150">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b57e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b57e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b57e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b57e-152">Request</span></span>
<span data-ttu-id="6b57e-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b57e-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="6b57e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b57e-154">Response</span></span>
<span data-ttu-id="6b57e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b57e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




