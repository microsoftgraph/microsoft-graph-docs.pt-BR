---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f97f16298c48b787977330781e3aa95e68e4d28a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861765"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="de214-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="de214-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="de214-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de214-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de214-105">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="de214-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de214-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de214-106">Prerequisites</span></span>
<span data-ttu-id="de214-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de214-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de214-109">Permission type</span></span>|<span data-ttu-id="de214-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de214-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de214-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de214-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de214-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de214-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de214-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de214-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de214-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de214-114">Not supported.</span></span>|
|<span data-ttu-id="de214-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de214-115">Application</span></span>|<span data-ttu-id="de214-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de214-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de214-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de214-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="de214-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de214-118">Request headers</span></span>
|<span data-ttu-id="de214-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de214-119">Header</span></span>|<span data-ttu-id="de214-120">Valor</span><span class="sxs-lookup"><span data-stu-id="de214-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de214-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de214-121">Authorization</span></span>|<span data-ttu-id="de214-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de214-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de214-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de214-123">Accept</span></span>|<span data-ttu-id="de214-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de214-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de214-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de214-125">Request body</span></span>
<span data-ttu-id="de214-126">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="de214-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="de214-127">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="de214-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="de214-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de214-128">Property</span></span>|<span data-ttu-id="de214-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="de214-129">Type</span></span>|<span data-ttu-id="de214-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="de214-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de214-131">id</span><span class="sxs-lookup"><span data-stu-id="de214-131">id</span></span>|<span data-ttu-id="de214-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de214-132">String</span></span>|<span data-ttu-id="de214-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de214-133">Key of the entity.</span></span>|
|<span data-ttu-id="de214-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de214-134">lastModifiedDateTime</span></span>|<span data-ttu-id="de214-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de214-135">DateTimeOffset</span></span>|<span data-ttu-id="de214-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="de214-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="de214-137">displayName</span><span class="sxs-lookup"><span data-stu-id="de214-137">displayName</span></span>|<span data-ttu-id="de214-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de214-138">String</span></span>|<span data-ttu-id="de214-139">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="de214-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="de214-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="de214-140">defaultLocale</span></span>|<span data-ttu-id="de214-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de214-141">String</span></span>|<span data-ttu-id="de214-142">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="de214-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="de214-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="de214-143">brandingOptions</span></span>|[<span data-ttu-id="de214-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="de214-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="de214-145">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="de214-145">The Message Template Branding Options.</span></span> <span data-ttu-id="de214-146">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="de214-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="de214-147">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="de214-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="de214-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="de214-148">Response</span></span>
<span data-ttu-id="de214-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de214-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de214-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de214-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="de214-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de214-151">Request</span></span>
<span data-ttu-id="de214-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de214-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de214-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="de214-153">Response</span></span>
<span data-ttu-id="de214-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de214-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



