---
title: Tipo de recurso notificationMessageTemplate
description: Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05db5042b43097f0ff48f4c744e3b4bcd82f691d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072988"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="d0529-105">Tipo de recurso notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="d0529-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0529-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0529-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0529-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0529-108">Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d0529-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="d0529-109">Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade".</span><span class="sxs-lookup"><span data-stu-id="d0529-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="d0529-110">Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.</span><span class="sxs-lookup"><span data-stu-id="d0529-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="d0529-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d0529-111">Methods</span></span>
|<span data-ttu-id="d0529-112">Método</span><span class="sxs-lookup"><span data-stu-id="d0529-112">Method</span></span>|<span data-ttu-id="d0529-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0529-113">Return Type</span></span>|<span data-ttu-id="d0529-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0529-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0529-115">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="d0529-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="d0529-116">Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d0529-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="d0529-117">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0529-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="d0529-118">Obter notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="d0529-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d0529-120">Ler propriedades e relações do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0529-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d0529-121">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="d0529-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d0529-123">Criar um novo objeto de [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0529-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d0529-124">Excluir notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="d0529-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0529-125">None</span></span>|<span data-ttu-id="d0529-126">Excluir um [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0529-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="d0529-127">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="d0529-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d0529-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d0529-129">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d0529-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d0529-130">Ação sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="d0529-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="d0529-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0529-131">None</span></span>|<span data-ttu-id="d0529-132">Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão</span><span class="sxs-lookup"><span data-stu-id="d0529-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="d0529-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0529-133">Properties</span></span>
|<span data-ttu-id="d0529-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0529-134">Property</span></span>|<span data-ttu-id="d0529-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0529-135">Type</span></span>|<span data-ttu-id="d0529-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0529-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0529-137">id</span><span class="sxs-lookup"><span data-stu-id="d0529-137">id</span></span>|<span data-ttu-id="d0529-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0529-138">String</span></span>|<span data-ttu-id="d0529-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d0529-139">Key of the entity.</span></span>|
|<span data-ttu-id="d0529-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0529-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d0529-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0529-141">DateTimeOffset</span></span>|<span data-ttu-id="d0529-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d0529-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d0529-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d0529-143">displayName</span></span>|<span data-ttu-id="d0529-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0529-144">String</span></span>|<span data-ttu-id="d0529-145">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="d0529-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="d0529-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="d0529-146">defaultLocale</span></span>|<span data-ttu-id="d0529-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0529-147">String</span></span>|<span data-ttu-id="d0529-148">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="d0529-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="d0529-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="d0529-149">brandingOptions</span></span>|[<span data-ttu-id="d0529-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="d0529-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="d0529-151">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="d0529-151">The Message Template Branding Options.</span></span> <span data-ttu-id="d0529-152">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="d0529-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="d0529-153">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="d0529-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0529-154">Relações</span><span class="sxs-lookup"><span data-stu-id="d0529-154">Relationships</span></span>
|<span data-ttu-id="d0529-155">Relação</span><span class="sxs-lookup"><span data-stu-id="d0529-155">Relationship</span></span>|<span data-ttu-id="d0529-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0529-156">Type</span></span>|<span data-ttu-id="d0529-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0529-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0529-158">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="d0529-158">localizedNotificationMessages</span></span>|<span data-ttu-id="d0529-159">Coleção [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d0529-159">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="d0529-160">A lista de mensagens localizadas para esse modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="d0529-160">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0529-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0529-161">JSON Representation</span></span>
<span data-ttu-id="d0529-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0529-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```









