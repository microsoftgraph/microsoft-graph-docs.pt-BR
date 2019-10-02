---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49ee38a00ea8cbc93e476f1f25be6790b94358a8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362839"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="d0f19-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0f19-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="d0f19-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0f19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f19-105">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0f19-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0f19-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0f19-106">Prerequisites</span></span>
<span data-ttu-id="d0f19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0f19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0f19-109">Permission type</span></span>|<span data-ttu-id="d0f19-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0f19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0f19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f19-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f19-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0f19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0f19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f19-114">Not supported.</span></span>|
|<span data-ttu-id="d0f19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0f19-115">Application</span></span>|<span data-ttu-id="d0f19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="d0f19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f19-118">Request headers</span></span>
|<span data-ttu-id="d0f19-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0f19-119">Header</span></span>|<span data-ttu-id="d0f19-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d0f19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0f19-121">Authorization</span></span>|<span data-ttu-id="d0f19-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0f19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0f19-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0f19-123">Accept</span></span>|<span data-ttu-id="d0f19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f19-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f19-125">Request body</span></span>
<span data-ttu-id="d0f19-126">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="d0f19-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="d0f19-127">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="d0f19-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="d0f19-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0f19-128">Property</span></span>|<span data-ttu-id="d0f19-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0f19-129">Type</span></span>|<span data-ttu-id="d0f19-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0f19-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f19-131">id</span><span class="sxs-lookup"><span data-stu-id="d0f19-131">id</span></span>|<span data-ttu-id="d0f19-132">String</span><span class="sxs-lookup"><span data-stu-id="d0f19-132">String</span></span>|<span data-ttu-id="d0f19-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d0f19-133">Key of the entity.</span></span>|
|<span data-ttu-id="d0f19-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f19-134">lastModifiedDateTime</span></span>|<span data-ttu-id="d0f19-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f19-135">DateTimeOffset</span></span>|<span data-ttu-id="d0f19-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d0f19-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d0f19-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d0f19-137">displayName</span></span>|<span data-ttu-id="d0f19-138">String</span><span class="sxs-lookup"><span data-stu-id="d0f19-138">String</span></span>|<span data-ttu-id="d0f19-139">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="d0f19-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="d0f19-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="d0f19-140">defaultLocale</span></span>|<span data-ttu-id="d0f19-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0f19-141">String</span></span>|<span data-ttu-id="d0f19-142">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="d0f19-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="d0f19-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="d0f19-143">brandingOptions</span></span>|[<span data-ttu-id="d0f19-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="d0f19-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="d0f19-145">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="d0f19-145">The Message Template Branding Options.</span></span> <span data-ttu-id="d0f19-146">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="d0f19-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="d0f19-147">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="d0f19-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0f19-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f19-148">Response</span></span>
<span data-ttu-id="d0f19-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f19-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f19-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0f19-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0f19-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f19-151">Request</span></span>
<span data-ttu-id="d0f19-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0f19-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0f19-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f19-153">Response</span></span>
<span data-ttu-id="d0f19-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0f19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




