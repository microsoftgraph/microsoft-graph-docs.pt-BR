---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da5833e5e357876410cb2e3494db24e2c950277c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984633"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="e80a8-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="e80a8-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="e80a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e80a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e80a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e80a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e80a8-106">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e80a8-106">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e80a8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e80a8-107">Prerequisites</span></span>
<span data-ttu-id="e80a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e80a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e80a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e80a8-110">Permission type</span></span>|<span data-ttu-id="e80a8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e80a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e80a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e80a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e80a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e80a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e80a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e80a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e80a8-115">Not supported.</span></span>|
|<span data-ttu-id="e80a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e80a8-116">Application</span></span>|<span data-ttu-id="e80a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e80a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e80a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e80a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="e80a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e80a8-119">Request headers</span></span>
|<span data-ttu-id="e80a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e80a8-120">Header</span></span>|<span data-ttu-id="e80a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e80a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e80a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e80a8-122">Authorization</span></span>|<span data-ttu-id="e80a8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e80a8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e80a8-124">Accept</span></span>|<span data-ttu-id="e80a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e80a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e80a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e80a8-126">Request body</span></span>
<span data-ttu-id="e80a8-127">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="e80a8-127">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="e80a8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="e80a8-128">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="e80a8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e80a8-129">Property</span></span>|<span data-ttu-id="e80a8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80a8-130">Type</span></span>|<span data-ttu-id="e80a8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e80a8-132">id</span><span class="sxs-lookup"><span data-stu-id="e80a8-132">id</span></span>|<span data-ttu-id="e80a8-133">String</span><span class="sxs-lookup"><span data-stu-id="e80a8-133">String</span></span>|<span data-ttu-id="e80a8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e80a8-134">Key of the entity.</span></span>|
|<span data-ttu-id="e80a8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e80a8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e80a8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e80a8-136">DateTimeOffset</span></span>|<span data-ttu-id="e80a8-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e80a8-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e80a8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e80a8-138">displayName</span></span>|<span data-ttu-id="e80a8-139">String</span><span class="sxs-lookup"><span data-stu-id="e80a8-139">String</span></span>|<span data-ttu-id="e80a8-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="e80a8-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="e80a8-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="e80a8-141">defaultLocale</span></span>|<span data-ttu-id="e80a8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e80a8-142">String</span></span>|<span data-ttu-id="e80a8-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="e80a8-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="e80a8-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="e80a8-144">brandingOptions</span></span>|[<span data-ttu-id="e80a8-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="e80a8-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="e80a8-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="e80a8-146">The Message Template Branding Options.</span></span> <span data-ttu-id="e80a8-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="e80a8-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="e80a8-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="e80a8-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="e80a8-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e80a8-149">roleScopeTagIds</span></span>|<span data-ttu-id="e80a8-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e80a8-150">String collection</span></span>|<span data-ttu-id="e80a8-151">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e80a8-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e80a8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80a8-152">Response</span></span>
<span data-ttu-id="e80a8-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e80a8-153">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e80a8-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e80a8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e80a8-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e80a8-155">Request</span></span>
<span data-ttu-id="e80a8-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e80a8-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
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

### <a name="response"></a><span data-ttu-id="e80a8-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80a8-157">Response</span></span>
<span data-ttu-id="e80a8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e80a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





