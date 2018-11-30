---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
ms.openlocfilehash: 013acd831979fdbb22eb67be66552b2d21d590b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041192"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="1b404-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="1b404-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="1b404-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b404-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b404-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b404-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b404-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b404-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b404-107">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1b404-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b404-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b404-108">Prerequisites</span></span>
<span data-ttu-id="1b404-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b404-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b404-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b404-111">Permission type</span></span>|<span data-ttu-id="1b404-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b404-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b404-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b404-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b404-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b404-116">Not supported.</span></span>|
|<span data-ttu-id="1b404-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b404-117">Application</span></span>|<span data-ttu-id="1b404-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b404-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b404-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="1b404-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-120">Request headers</span></span>
|<span data-ttu-id="1b404-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b404-121">Header</span></span>|<span data-ttu-id="1b404-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b404-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b404-123">Authorization</span></span>|<span data-ttu-id="1b404-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b404-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b404-125">Accept</span></span>|<span data-ttu-id="1b404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b404-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-127">Request body</span></span>
<span data-ttu-id="1b404-128">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="1b404-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="1b404-129">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="1b404-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="1b404-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b404-130">Property</span></span>|<span data-ttu-id="1b404-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b404-131">Type</span></span>|<span data-ttu-id="1b404-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b404-133">id</span><span class="sxs-lookup"><span data-stu-id="1b404-133">id</span></span>|<span data-ttu-id="1b404-134">String</span><span class="sxs-lookup"><span data-stu-id="1b404-134">String</span></span>|<span data-ttu-id="1b404-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b404-135">Key of the entity.</span></span>|
|<span data-ttu-id="1b404-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b404-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b404-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b404-137">DateTimeOffset</span></span>|<span data-ttu-id="1b404-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1b404-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1b404-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1b404-139">displayName</span></span>|<span data-ttu-id="1b404-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-140">String</span></span>|<span data-ttu-id="1b404-141">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="1b404-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="1b404-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="1b404-142">defaultLocale</span></span>|<span data-ttu-id="1b404-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-143">String</span></span>|<span data-ttu-id="1b404-144">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="1b404-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="1b404-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="1b404-145">brandingOptions</span></span>|[<span data-ttu-id="1b404-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="1b404-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="1b404-147">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="1b404-147">The Message Template Branding Options.</span></span> <span data-ttu-id="1b404-148">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="1b404-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="1b404-149">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="1b404-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="1b404-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b404-150">roleScopeTagIds</span></span>|<span data-ttu-id="1b404-151">String collection</span><span class="sxs-lookup"><span data-stu-id="1b404-151">String collection</span></span>|<span data-ttu-id="1b404-152">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b404-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1b404-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b404-153">Response</span></span>
<span data-ttu-id="1b404-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b404-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b404-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b404-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b404-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-156">Request</span></span>
<span data-ttu-id="1b404-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b404-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1b404-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b404-158">Response</span></span>
<span data-ttu-id="1b404-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b404-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





