---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ba404f8a0c738891a9791c3f0875ecc2d4d4d99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994275"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="e45a3-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="e45a3-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="e45a3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e45a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e45a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e45a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45a3-106">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e45a3-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e45a3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e45a3-107">Prerequisites</span></span>
<span data-ttu-id="e45a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e45a3-110">Permission type</span></span>|<span data-ttu-id="e45a3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e45a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e45a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e45a3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45a3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e45a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e45a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e45a3-115">Not supported.</span></span>|
|<span data-ttu-id="e45a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e45a3-116">Application</span></span>|<span data-ttu-id="e45a3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e45a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e45a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="e45a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e45a3-119">Request headers</span></span>
|<span data-ttu-id="e45a3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e45a3-120">Header</span></span>|<span data-ttu-id="e45a3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e45a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e45a3-122">Authorization</span></span>|<span data-ttu-id="e45a3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e45a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45a3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e45a3-124">Accept</span></span>|<span data-ttu-id="e45a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e45a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45a3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e45a3-126">Request body</span></span>
<span data-ttu-id="e45a3-127">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e45a3-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="e45a3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e45a3-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="e45a3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e45a3-129">Property</span></span>|<span data-ttu-id="e45a3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e45a3-130">Type</span></span>|<span data-ttu-id="e45a3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e45a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45a3-132">id</span><span class="sxs-lookup"><span data-stu-id="e45a3-132">id</span></span>|<span data-ttu-id="e45a3-133">String</span><span class="sxs-lookup"><span data-stu-id="e45a3-133">String</span></span>|<span data-ttu-id="e45a3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e45a3-134">Key of the entity.</span></span>|
|<span data-ttu-id="e45a3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e45a3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e45a3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45a3-136">DateTimeOffset</span></span>|<span data-ttu-id="e45a3-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e45a3-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e45a3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e45a3-138">displayName</span></span>|<span data-ttu-id="e45a3-139">String</span><span class="sxs-lookup"><span data-stu-id="e45a3-139">String</span></span>|<span data-ttu-id="e45a3-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="e45a3-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="e45a3-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="e45a3-141">defaultLocale</span></span>|<span data-ttu-id="e45a3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e45a3-142">String</span></span>|<span data-ttu-id="e45a3-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="e45a3-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="e45a3-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="e45a3-144">brandingOptions</span></span>|[<span data-ttu-id="e45a3-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="e45a3-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="e45a3-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="e45a3-146">The Message Template Branding Options.</span></span> <span data-ttu-id="e45a3-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="e45a3-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="e45a3-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="e45a3-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="e45a3-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e45a3-149">roleScopeTagIds</span></span>|<span data-ttu-id="e45a3-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e45a3-150">String collection</span></span>|<span data-ttu-id="e45a3-151">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e45a3-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e45a3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45a3-152">Response</span></span>
<span data-ttu-id="e45a3-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e45a3-153">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45a3-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e45a3-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45a3-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e45a3-155">Request</span></span>
<span data-ttu-id="e45a3-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e45a3-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e45a3-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45a3-157">Response</span></span>
<span data-ttu-id="e45a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e45a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





