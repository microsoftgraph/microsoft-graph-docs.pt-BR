---
title: Atualizar notificationMessageTemplate
description: Atualizar as propriedades de um objeto notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bcf7fe7800ba7023d230a7d82755e3f36e2b06f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975592"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="a9ad7-103">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a9ad7-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="a9ad7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9ad7-105">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a9ad7-105">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9ad7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9ad7-106">Prerequisites</span></span>
<span data-ttu-id="a9ad7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9ad7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9ad7-109">Permission type</span></span>|<span data-ttu-id="a9ad7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9ad7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9ad7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9ad7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9ad7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ad7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9ad7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9ad7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9ad7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-114">Not supported.</span></span>|
|<span data-ttu-id="a9ad7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9ad7-115">Application</span></span>|<span data-ttu-id="a9ad7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9ad7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9ad7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="a9ad7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ad7-118">Request headers</span></span>
|<span data-ttu-id="a9ad7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9ad7-119">Header</span></span>|<span data-ttu-id="a9ad7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9ad7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9ad7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9ad7-121">Authorization</span></span>|<span data-ttu-id="a9ad7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9ad7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9ad7-123">Accept</span></span>|<span data-ttu-id="a9ad7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9ad7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9ad7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ad7-125">Request body</span></span>
<span data-ttu-id="a9ad7-126">No corpo da solicitação, forneça uma representação JSON do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a9ad7-126">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="a9ad7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a9ad7-127">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="a9ad7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9ad7-128">Property</span></span>|<span data-ttu-id="a9ad7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9ad7-129">Type</span></span>|<span data-ttu-id="a9ad7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ad7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9ad7-131">id</span><span class="sxs-lookup"><span data-stu-id="a9ad7-131">id</span></span>|<span data-ttu-id="a9ad7-132">String</span><span class="sxs-lookup"><span data-stu-id="a9ad7-132">String</span></span>|<span data-ttu-id="a9ad7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-133">Key of the entity.</span></span>|
|<span data-ttu-id="a9ad7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9ad7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="a9ad7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9ad7-135">DateTimeOffset</span></span>|<span data-ttu-id="a9ad7-136">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a9ad7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a9ad7-137">displayName</span></span>|<span data-ttu-id="a9ad7-138">String</span><span class="sxs-lookup"><span data-stu-id="a9ad7-138">String</span></span>|<span data-ttu-id="a9ad7-139">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="a9ad7-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="a9ad7-140">defaultLocale</span></span>|<span data-ttu-id="a9ad7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9ad7-141">String</span></span>|<span data-ttu-id="a9ad7-142">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="a9ad7-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="a9ad7-143">brandingOptions</span></span>|[<span data-ttu-id="a9ad7-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="a9ad7-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="a9ad7-145">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-145">The Message Template Branding Options.</span></span> <span data-ttu-id="a9ad7-146">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="a9ad7-147">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9ad7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ad7-148">Response</span></span>
<span data-ttu-id="a9ad7-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-149">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ad7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9ad7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9ad7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ad7-151">Request</span></span>
<span data-ttu-id="a9ad7-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="a9ad7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ad7-153">Response</span></span>
<span data-ttu-id="a9ad7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9ad7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



