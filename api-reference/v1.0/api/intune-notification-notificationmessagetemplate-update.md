---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 288361a17d4bc9ec73f879b986d9066cebd7f21d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967909"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="ef6f4-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ef6f4-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="ef6f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef6f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef6f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef6f4-106">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ef6f4-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef6f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef6f4-107">Prerequisites</span></span>
<span data-ttu-id="ef6f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef6f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef6f4-110">Permission type</span></span>|<span data-ttu-id="ef6f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef6f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef6f4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef6f4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef6f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef6f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-115">Not supported.</span></span>|
|<span data-ttu-id="ef6f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef6f4-116">Application</span></span>|<span data-ttu-id="ef6f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef6f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef6f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="ef6f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef6f4-119">Request headers</span></span>
|<span data-ttu-id="ef6f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef6f4-120">Header</span></span>|<span data-ttu-id="ef6f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef6f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef6f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef6f4-122">Authorization</span></span>|<span data-ttu-id="ef6f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef6f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef6f4-124">Accept</span></span>|<span data-ttu-id="ef6f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef6f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef6f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef6f4-126">Request body</span></span>
<span data-ttu-id="ef6f4-127">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ef6f4-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="ef6f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ef6f4-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="ef6f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef6f4-129">Property</span></span>|<span data-ttu-id="ef6f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef6f4-130">Type</span></span>|<span data-ttu-id="ef6f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef6f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef6f4-132">id</span><span class="sxs-lookup"><span data-stu-id="ef6f4-132">id</span></span>|<span data-ttu-id="ef6f4-133">String</span><span class="sxs-lookup"><span data-stu-id="ef6f4-133">String</span></span>|<span data-ttu-id="ef6f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-134">Key of the entity.</span></span>|
|<span data-ttu-id="ef6f4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6f4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ef6f4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6f4-136">DateTimeOffset</span></span>|<span data-ttu-id="ef6f4-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ef6f4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ef6f4-138">displayName</span></span>|<span data-ttu-id="ef6f4-139">String</span><span class="sxs-lookup"><span data-stu-id="ef6f4-139">String</span></span>|<span data-ttu-id="ef6f4-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="ef6f4-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="ef6f4-141">defaultLocale</span></span>|<span data-ttu-id="ef6f4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef6f4-142">String</span></span>|<span data-ttu-id="ef6f4-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="ef6f4-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="ef6f4-144">brandingOptions</span></span>|[<span data-ttu-id="ef6f4-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="ef6f4-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="ef6f4-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-146">The Message Template Branding Options.</span></span> <span data-ttu-id="ef6f4-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="ef6f4-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef6f4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef6f4-149">Response</span></span>
<span data-ttu-id="ef6f4-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-150">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef6f4-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef6f4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef6f4-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef6f4-152">Request</span></span>
<span data-ttu-id="ef6f4-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef6f4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef6f4-154">Response</span></span>
<span data-ttu-id="ef6f4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef6f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









