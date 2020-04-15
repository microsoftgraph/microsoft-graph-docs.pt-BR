---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11aa54ec5548fdf63c9bae467fa2176ad1907038
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452929"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="a873d-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a873d-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="a873d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a873d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a873d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a873d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a873d-106">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a873d-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a873d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a873d-107">Prerequisites</span></span>
<span data-ttu-id="a873d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a873d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a873d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a873d-110">Permission type</span></span>|<span data-ttu-id="a873d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a873d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a873d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a873d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a873d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a873d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a873d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a873d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a873d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a873d-115">Not supported.</span></span>|
|<span data-ttu-id="a873d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a873d-116">Application</span></span>|<span data-ttu-id="a873d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a873d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a873d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a873d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="a873d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a873d-119">Request headers</span></span>
|<span data-ttu-id="a873d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a873d-120">Header</span></span>|<span data-ttu-id="a873d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a873d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a873d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a873d-122">Authorization</span></span>|<span data-ttu-id="a873d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a873d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a873d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a873d-124">Accept</span></span>|<span data-ttu-id="a873d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a873d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a873d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a873d-126">Request body</span></span>
<span data-ttu-id="a873d-127">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a873d-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="a873d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a873d-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="a873d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a873d-129">Property</span></span>|<span data-ttu-id="a873d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a873d-130">Type</span></span>|<span data-ttu-id="a873d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a873d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a873d-132">id</span><span class="sxs-lookup"><span data-stu-id="a873d-132">id</span></span>|<span data-ttu-id="a873d-133">String</span><span class="sxs-lookup"><span data-stu-id="a873d-133">String</span></span>|<span data-ttu-id="a873d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a873d-134">Key of the entity.</span></span>|
|<span data-ttu-id="a873d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a873d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a873d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a873d-136">DateTimeOffset</span></span>|<span data-ttu-id="a873d-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a873d-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a873d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a873d-138">displayName</span></span>|<span data-ttu-id="a873d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a873d-139">String</span></span>|<span data-ttu-id="a873d-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="a873d-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="a873d-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="a873d-141">defaultLocale</span></span>|<span data-ttu-id="a873d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a873d-142">String</span></span>|<span data-ttu-id="a873d-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a873d-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="a873d-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="a873d-144">brandingOptions</span></span>|[<span data-ttu-id="a873d-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="a873d-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="a873d-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="a873d-146">The Message Template Branding Options.</span></span> <span data-ttu-id="a873d-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="a873d-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="a873d-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="a873d-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="a873d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a873d-149">Response</span></span>
<span data-ttu-id="a873d-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a873d-150">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a873d-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a873d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="a873d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a873d-152">Request</span></span>
<span data-ttu-id="a873d-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a873d-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a873d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a873d-154">Response</span></span>
<span data-ttu-id="a873d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a873d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






