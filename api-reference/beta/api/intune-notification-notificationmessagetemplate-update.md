---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 288877244d15cffda434981720b4107009122b66
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941957"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="3a70f-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="3a70f-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="3a70f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a70f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a70f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a70f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a70f-106">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="3a70f-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a70f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a70f-107">Prerequisites</span></span>
<span data-ttu-id="3a70f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a70f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a70f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a70f-110">Permission type</span></span>|<span data-ttu-id="3a70f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a70f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a70f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a70f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a70f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a70f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a70f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a70f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a70f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a70f-115">Not supported.</span></span>|
|<span data-ttu-id="3a70f-116">Application</span><span class="sxs-lookup"><span data-stu-id="3a70f-116">Application</span></span>|<span data-ttu-id="3a70f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a70f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a70f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a70f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="3a70f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a70f-119">Request headers</span></span>
|<span data-ttu-id="3a70f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a70f-120">Header</span></span>|<span data-ttu-id="3a70f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a70f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a70f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a70f-122">Authorization</span></span>|<span data-ttu-id="3a70f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a70f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a70f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a70f-124">Accept</span></span>|<span data-ttu-id="3a70f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a70f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a70f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a70f-126">Request body</span></span>
<span data-ttu-id="3a70f-127">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="3a70f-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="3a70f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="3a70f-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="3a70f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a70f-129">Property</span></span>|<span data-ttu-id="3a70f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a70f-130">Type</span></span>|<span data-ttu-id="3a70f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a70f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a70f-132">id</span><span class="sxs-lookup"><span data-stu-id="3a70f-132">id</span></span>|<span data-ttu-id="3a70f-133">String</span><span class="sxs-lookup"><span data-stu-id="3a70f-133">String</span></span>|<span data-ttu-id="3a70f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3a70f-134">Key of the entity.</span></span>|
|<span data-ttu-id="3a70f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a70f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3a70f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a70f-136">DateTimeOffset</span></span>|<span data-ttu-id="3a70f-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3a70f-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3a70f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3a70f-138">displayName</span></span>|<span data-ttu-id="3a70f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a70f-139">String</span></span>|<span data-ttu-id="3a70f-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="3a70f-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="3a70f-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="3a70f-141">defaultLocale</span></span>|<span data-ttu-id="3a70f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a70f-142">String</span></span>|<span data-ttu-id="3a70f-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="3a70f-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="3a70f-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="3a70f-144">brandingOptions</span></span>|[<span data-ttu-id="3a70f-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="3a70f-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="3a70f-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="3a70f-146">The Message Template Branding Options.</span></span> <span data-ttu-id="3a70f-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="3a70f-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="3a70f-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="3a70f-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="3a70f-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a70f-149">roleScopeTagIds</span></span>|<span data-ttu-id="3a70f-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a70f-150">String collection</span></span>|<span data-ttu-id="3a70f-151">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3a70f-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3a70f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a70f-152">Response</span></span>
<span data-ttu-id="3a70f-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a70f-153">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a70f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a70f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a70f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a70f-155">Request</span></span>
<span data-ttu-id="3a70f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a70f-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a70f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a70f-157">Response</span></span>
<span data-ttu-id="3a70f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a70f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





