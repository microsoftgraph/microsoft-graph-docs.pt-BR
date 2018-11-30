---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
ms.openlocfilehash: 9d1d54e992a51344c3310ccf3d63890cd60c15c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007018"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="7403c-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="7403c-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="7403c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7403c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7403c-105">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="7403c-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7403c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7403c-106">Prerequisites</span></span>
<span data-ttu-id="7403c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7403c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7403c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7403c-109">Permission type</span></span>|<span data-ttu-id="7403c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7403c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7403c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7403c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7403c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7403c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7403c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7403c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7403c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7403c-114">Not supported.</span></span>|
|<span data-ttu-id="7403c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7403c-115">Application</span></span>|<span data-ttu-id="7403c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7403c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7403c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7403c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="7403c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7403c-118">Request headers</span></span>
|<span data-ttu-id="7403c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7403c-119">Header</span></span>|<span data-ttu-id="7403c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7403c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7403c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7403c-121">Authorization</span></span>|<span data-ttu-id="7403c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7403c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7403c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7403c-123">Accept</span></span>|<span data-ttu-id="7403c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7403c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7403c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7403c-125">Request body</span></span>
<span data-ttu-id="7403c-126">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="7403c-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="7403c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="7403c-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="7403c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7403c-128">Property</span></span>|<span data-ttu-id="7403c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7403c-129">Type</span></span>|<span data-ttu-id="7403c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7403c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7403c-131">id</span><span class="sxs-lookup"><span data-stu-id="7403c-131">id</span></span>|<span data-ttu-id="7403c-132">String</span><span class="sxs-lookup"><span data-stu-id="7403c-132">String</span></span>|<span data-ttu-id="7403c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7403c-133">Key of the entity.</span></span>|
|<span data-ttu-id="7403c-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7403c-134">lastModifiedDateTime</span></span>|<span data-ttu-id="7403c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7403c-135">DateTimeOffset</span></span>|<span data-ttu-id="7403c-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7403c-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7403c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7403c-137">displayName</span></span>|<span data-ttu-id="7403c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7403c-138">String</span></span>|<span data-ttu-id="7403c-139">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="7403c-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="7403c-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="7403c-140">defaultLocale</span></span>|<span data-ttu-id="7403c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7403c-141">String</span></span>|<span data-ttu-id="7403c-142">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="7403c-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="7403c-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="7403c-143">brandingOptions</span></span>|[<span data-ttu-id="7403c-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="7403c-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="7403c-145">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="7403c-145">The Message Template Branding Options.</span></span> <span data-ttu-id="7403c-146">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="7403c-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="7403c-147">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="7403c-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="7403c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7403c-148">Response</span></span>
<span data-ttu-id="7403c-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7403c-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7403c-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7403c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="7403c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7403c-151">Request</span></span>
<span data-ttu-id="7403c-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7403c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="7403c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7403c-153">Response</span></span>
<span data-ttu-id="7403c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7403c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



