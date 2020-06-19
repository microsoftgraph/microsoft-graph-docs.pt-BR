---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbccbb8e464d3009304bcf84a1677235bab4fe28
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791865"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="eb3ef-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="eb3ef-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="eb3ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb3ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb3ef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb3ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb3ef-107">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="eb3ef-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb3ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb3ef-108">Prerequisites</span></span>
<span data-ttu-id="eb3ef-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="eb3ef-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb3ef-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb3ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb3ef-111">Permission type</span></span>|<span data-ttu-id="eb3ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb3ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb3ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb3ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb3ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb3ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb3ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb3ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-116">Not supported.</span></span>|
|<span data-ttu-id="eb3ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb3ef-117">Application</span></span>|<span data-ttu-id="eb3ef-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3ef-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb3ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb3ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="eb3ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb3ef-120">Request headers</span></span>
|<span data-ttu-id="eb3ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb3ef-121">Header</span></span>|<span data-ttu-id="eb3ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb3ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb3ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb3ef-123">Authorization</span></span>|<span data-ttu-id="eb3ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb3ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb3ef-125">Accept</span></span>|<span data-ttu-id="eb3ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb3ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb3ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb3ef-127">Request body</span></span>
<span data-ttu-id="eb3ef-128">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="eb3ef-129">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="eb3ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb3ef-130">Property</span></span>|<span data-ttu-id="eb3ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb3ef-131">Type</span></span>|<span data-ttu-id="eb3ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb3ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb3ef-133">id</span><span class="sxs-lookup"><span data-stu-id="eb3ef-133">id</span></span>|<span data-ttu-id="eb3ef-134">String</span><span class="sxs-lookup"><span data-stu-id="eb3ef-134">String</span></span>|<span data-ttu-id="eb3ef-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-135">Key of the entity.</span></span>|
|<span data-ttu-id="eb3ef-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb3ef-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eb3ef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb3ef-137">DateTimeOffset</span></span>|<span data-ttu-id="eb3ef-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="eb3ef-139">displayName</span><span class="sxs-lookup"><span data-stu-id="eb3ef-139">displayName</span></span>|<span data-ttu-id="eb3ef-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb3ef-140">String</span></span>|<span data-ttu-id="eb3ef-141">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="eb3ef-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="eb3ef-142">defaultLocale</span></span>|<span data-ttu-id="eb3ef-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb3ef-143">String</span></span>|<span data-ttu-id="eb3ef-144">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="eb3ef-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="eb3ef-145">brandingOptions</span></span>|[<span data-ttu-id="eb3ef-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="eb3ef-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="eb3ef-147">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-147">The Message Template Branding Options.</span></span> <span data-ttu-id="eb3ef-148">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="eb3ef-149">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="eb3ef-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eb3ef-150">roleScopeTagIds</span></span>|<span data-ttu-id="eb3ef-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb3ef-151">String collection</span></span>|<span data-ttu-id="eb3ef-152">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="eb3ef-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb3ef-153">Response</span></span>
<span data-ttu-id="eb3ef-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb3ef-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb3ef-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb3ef-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb3ef-156">Request</span></span>
<span data-ttu-id="eb3ef-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb3ef-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb3ef-158">Response</span></span>
<span data-ttu-id="eb3ef-159">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-159">Here is an example of the response.</span></span> <span data-ttu-id="eb3ef-160">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eb3ef-161">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="eb3ef-161">All of the properties will be returned from an actual call.</span></span>
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



