---
title: Criar notificationMessageTemplate
description: Criar um novo objeto notificationMessageTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bb8ae2079920b8ee7ce19065a3c857da063675c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512759"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="76aac-103">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="76aac-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="76aac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76aac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76aac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76aac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76aac-106">Criar um novo objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="76aac-106">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76aac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76aac-107">Prerequisites</span></span>
<span data-ttu-id="76aac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76aac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76aac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76aac-110">Permission type</span></span>|<span data-ttu-id="76aac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76aac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76aac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76aac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76aac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76aac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="76aac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76aac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76aac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76aac-115">Not supported.</span></span>|
|<span data-ttu-id="76aac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76aac-116">Application</span></span>|<span data-ttu-id="76aac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76aac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76aac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76aac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="76aac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76aac-119">Request headers</span></span>
|<span data-ttu-id="76aac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76aac-120">Header</span></span>|<span data-ttu-id="76aac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76aac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76aac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76aac-122">Authorization</span></span>|<span data-ttu-id="76aac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76aac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76aac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76aac-124">Accept</span></span>|<span data-ttu-id="76aac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76aac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76aac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76aac-126">Request body</span></span>
<span data-ttu-id="76aac-127">No corpo da solicitação, forneça uma representação JSON do objeto notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="76aac-127">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="76aac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="76aac-128">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="76aac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76aac-129">Property</span></span>|<span data-ttu-id="76aac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="76aac-130">Type</span></span>|<span data-ttu-id="76aac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="76aac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76aac-132">id</span><span class="sxs-lookup"><span data-stu-id="76aac-132">id</span></span>|<span data-ttu-id="76aac-133">String</span><span class="sxs-lookup"><span data-stu-id="76aac-133">String</span></span>|<span data-ttu-id="76aac-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76aac-134">Key of the entity.</span></span>|
|<span data-ttu-id="76aac-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76aac-135">lastModifiedDateTime</span></span>|<span data-ttu-id="76aac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76aac-136">DateTimeOffset</span></span>|<span data-ttu-id="76aac-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76aac-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="76aac-138">displayName</span><span class="sxs-lookup"><span data-stu-id="76aac-138">displayName</span></span>|<span data-ttu-id="76aac-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76aac-139">String</span></span>|<span data-ttu-id="76aac-140">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="76aac-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="76aac-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="76aac-141">defaultLocale</span></span>|<span data-ttu-id="76aac-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76aac-142">String</span></span>|<span data-ttu-id="76aac-143">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="76aac-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="76aac-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="76aac-144">brandingOptions</span></span>|[<span data-ttu-id="76aac-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="76aac-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="76aac-146">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="76aac-146">The Message Template Branding Options.</span></span> <span data-ttu-id="76aac-147">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="76aac-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="76aac-148">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="76aac-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="76aac-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="76aac-149">Response</span></span>
<span data-ttu-id="76aac-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76aac-150">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76aac-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76aac-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="76aac-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76aac-152">Request</span></span>
<span data-ttu-id="76aac-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76aac-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76aac-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="76aac-154">Response</span></span>
<span data-ttu-id="76aac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76aac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




