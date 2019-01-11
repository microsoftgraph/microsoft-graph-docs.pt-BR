---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 42eee498a1763110e7a0fcc622adaebda642562b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874050"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="415cf-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="415cf-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="415cf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="415cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="415cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="415cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="415cf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="415cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="415cf-107">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="415cf-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="415cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="415cf-108">Prerequisites</span></span>
<span data-ttu-id="415cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="415cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="415cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="415cf-111">Permission type</span></span>|<span data-ttu-id="415cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="415cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="415cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="415cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="415cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="415cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="415cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="415cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="415cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="415cf-116">Not supported.</span></span>|
|<span data-ttu-id="415cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="415cf-117">Application</span></span>|<span data-ttu-id="415cf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="415cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="415cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="415cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="415cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="415cf-120">Request headers</span></span>
|<span data-ttu-id="415cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="415cf-121">Header</span></span>|<span data-ttu-id="415cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="415cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="415cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="415cf-123">Authorization</span></span>|<span data-ttu-id="415cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="415cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="415cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="415cf-125">Accept</span></span>|<span data-ttu-id="415cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="415cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="415cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="415cf-127">Request body</span></span>
<span data-ttu-id="415cf-128">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="415cf-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="415cf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="415cf-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="415cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="415cf-130">Property</span></span>|<span data-ttu-id="415cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="415cf-131">Type</span></span>|<span data-ttu-id="415cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="415cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415cf-133">id</span><span class="sxs-lookup"><span data-stu-id="415cf-133">id</span></span>|<span data-ttu-id="415cf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="415cf-134">String</span></span>|<span data-ttu-id="415cf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="415cf-135">Key of the entity.</span></span>|
|<span data-ttu-id="415cf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="415cf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="415cf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="415cf-137">DateTimeOffset</span></span>|<span data-ttu-id="415cf-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="415cf-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="415cf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="415cf-139">displayName</span></span>|<span data-ttu-id="415cf-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="415cf-140">String</span></span>|<span data-ttu-id="415cf-141">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="415cf-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="415cf-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="415cf-142">defaultLocale</span></span>|<span data-ttu-id="415cf-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="415cf-143">String</span></span>|<span data-ttu-id="415cf-144">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="415cf-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="415cf-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="415cf-145">brandingOptions</span></span>|[<span data-ttu-id="415cf-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="415cf-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="415cf-147">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="415cf-147">The Message Template Branding Options.</span></span> <span data-ttu-id="415cf-148">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="415cf-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="415cf-149">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="415cf-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="415cf-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="415cf-150">roleScopeTagIds</span></span>|<span data-ttu-id="415cf-151">String collection</span><span class="sxs-lookup"><span data-stu-id="415cf-151">String collection</span></span>|<span data-ttu-id="415cf-152">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="415cf-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="415cf-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="415cf-153">Response</span></span>
<span data-ttu-id="415cf-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="415cf-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="415cf-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="415cf-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="415cf-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="415cf-156">Request</span></span>
<span data-ttu-id="415cf-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="415cf-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="415cf-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="415cf-158">Response</span></span>
<span data-ttu-id="415cf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="415cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





