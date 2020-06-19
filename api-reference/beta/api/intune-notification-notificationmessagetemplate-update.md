---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c2b3db6a3f23d6187a9f78340d2d6f4de3802db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791858"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="0ec41-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="0ec41-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="0ec41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ec41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ec41-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ec41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ec41-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ec41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ec41-107">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0ec41-107">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ec41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ec41-108">Prerequisites</span></span>
<span data-ttu-id="0ec41-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0ec41-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0ec41-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec41-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ec41-111">Permission type</span></span>|<span data-ttu-id="0ec41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ec41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ec41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ec41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ec41-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ec41-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ec41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ec41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ec41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec41-116">Not supported.</span></span>|
|<span data-ttu-id="0ec41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ec41-117">Application</span></span>|<span data-ttu-id="0ec41-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ec41-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ec41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="0ec41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec41-120">Request headers</span></span>
|<span data-ttu-id="0ec41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ec41-121">Header</span></span>|<span data-ttu-id="0ec41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ec41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ec41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ec41-123">Authorization</span></span>|<span data-ttu-id="0ec41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ec41-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ec41-125">Accept</span></span>|<span data-ttu-id="0ec41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ec41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ec41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec41-127">Request body</span></span>
<span data-ttu-id="0ec41-128">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0ec41-128">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="0ec41-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0ec41-129">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="0ec41-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ec41-130">Property</span></span>|<span data-ttu-id="0ec41-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec41-131">Type</span></span>|<span data-ttu-id="0ec41-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ec41-133">id</span><span class="sxs-lookup"><span data-stu-id="0ec41-133">id</span></span>|<span data-ttu-id="0ec41-134">String</span><span class="sxs-lookup"><span data-stu-id="0ec41-134">String</span></span>|<span data-ttu-id="0ec41-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ec41-135">Key of the entity.</span></span>|
|<span data-ttu-id="0ec41-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ec41-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ec41-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ec41-137">DateTimeOffset</span></span>|<span data-ttu-id="0ec41-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0ec41-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0ec41-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0ec41-139">displayName</span></span>|<span data-ttu-id="0ec41-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ec41-140">String</span></span>|<span data-ttu-id="0ec41-141">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="0ec41-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="0ec41-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="0ec41-142">defaultLocale</span></span>|<span data-ttu-id="0ec41-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ec41-143">String</span></span>|<span data-ttu-id="0ec41-144">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0ec41-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="0ec41-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="0ec41-145">brandingOptions</span></span>|[<span data-ttu-id="0ec41-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="0ec41-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="0ec41-147">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="0ec41-147">The Message Template Branding Options.</span></span> <span data-ttu-id="0ec41-148">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="0ec41-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="0ec41-149">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="0ec41-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="0ec41-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ec41-150">roleScopeTagIds</span></span>|<span data-ttu-id="0ec41-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ec41-151">String collection</span></span>|<span data-ttu-id="0ec41-152">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0ec41-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="0ec41-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec41-153">Response</span></span>
<span data-ttu-id="0ec41-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec41-154">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ec41-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ec41-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ec41-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec41-156">Request</span></span>
<span data-ttu-id="0ec41-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec41-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ec41-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec41-158">Response</span></span>
<span data-ttu-id="0ec41-159">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="0ec41-159">Here is an example of the response.</span></span> <span data-ttu-id="0ec41-160">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="0ec41-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0ec41-161">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0ec41-161">All of the properties will be returned from an actual call.</span></span>
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



