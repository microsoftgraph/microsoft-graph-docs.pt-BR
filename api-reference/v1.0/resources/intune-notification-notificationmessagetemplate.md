---
title: Tipo de recurso notificationMessageTemplate
description: Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bdc400a84f51fa11f3d70b28fd21973fd1cf663c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459622"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="ec6d2-105">Tipo de recurso notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="ec6d2-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec6d2-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec6d2-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec6d2-108">Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="ec6d2-109">Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade".</span><span class="sxs-lookup"><span data-stu-id="ec6d2-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="ec6d2-110">Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="ec6d2-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec6d2-111">Methods</span></span>
|<span data-ttu-id="ec6d2-112">Método</span><span class="sxs-lookup"><span data-stu-id="ec6d2-112">Method</span></span>|<span data-ttu-id="ec6d2-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec6d2-113">Return Type</span></span>|<span data-ttu-id="ec6d2-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec6d2-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec6d2-115">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="ec6d2-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="ec6d2-116">Conjunto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ec6d2-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="ec6d2-117">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ec6d2-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="ec6d2-118">Obter notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="ec6d2-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec6d2-120">Ler propriedades e relações do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ec6d2-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec6d2-121">Criar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="ec6d2-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec6d2-123">Criar um novo objeto de [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ec6d2-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec6d2-124">Excluir notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="ec6d2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec6d2-125">None</span></span>|<span data-ttu-id="ec6d2-126">Excluir um [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ec6d2-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="ec6d2-127">Atualizar notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="ec6d2-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec6d2-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec6d2-129">Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ec6d2-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec6d2-130">Ação sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="ec6d2-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="ec6d2-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec6d2-131">None</span></span>|<span data-ttu-id="ec6d2-132">Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão</span><span class="sxs-lookup"><span data-stu-id="ec6d2-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="ec6d2-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec6d2-133">Properties</span></span>
|<span data-ttu-id="ec6d2-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec6d2-134">Property</span></span>|<span data-ttu-id="ec6d2-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec6d2-135">Type</span></span>|<span data-ttu-id="ec6d2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec6d2-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec6d2-137">id</span><span class="sxs-lookup"><span data-stu-id="ec6d2-137">id</span></span>|<span data-ttu-id="ec6d2-138">String</span><span class="sxs-lookup"><span data-stu-id="ec6d2-138">String</span></span>|<span data-ttu-id="ec6d2-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-139">Key of the entity.</span></span>|
|<span data-ttu-id="ec6d2-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec6d2-140">lastModifiedDateTime</span></span>|<span data-ttu-id="ec6d2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec6d2-141">DateTimeOffset</span></span>|<span data-ttu-id="ec6d2-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ec6d2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ec6d2-143">displayName</span></span>|<span data-ttu-id="ec6d2-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec6d2-144">String</span></span>|<span data-ttu-id="ec6d2-145">Nome de exibição do modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="ec6d2-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="ec6d2-146">defaultLocale</span></span>|<span data-ttu-id="ec6d2-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec6d2-147">String</span></span>|<span data-ttu-id="ec6d2-148">A localidade padrão para fallback quando a localidade solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="ec6d2-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="ec6d2-149">brandingOptions</span></span>|[<span data-ttu-id="ec6d2-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="ec6d2-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="ec6d2-151">As opções de identidade visual do modelo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-151">The Message Template Branding Options.</span></span> <span data-ttu-id="ec6d2-152">A identidade visual é definida no Console do administrador do Intune.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="ec6d2-153">Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec6d2-154">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="ec6d2-154">Relationships</span></span>
|<span data-ttu-id="ec6d2-155">Relação</span><span class="sxs-lookup"><span data-stu-id="ec6d2-155">Relationship</span></span>|<span data-ttu-id="ec6d2-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec6d2-156">Type</span></span>|<span data-ttu-id="ec6d2-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec6d2-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec6d2-158">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="ec6d2-158">localizedNotificationMessages</span></span>|<span data-ttu-id="ec6d2-159">Coleção [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="ec6d2-159">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="ec6d2-160">A lista de mensagens localizadas para esse modelo de mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-160">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec6d2-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec6d2-161">JSON Representation</span></span>
<span data-ttu-id="ec6d2-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec6d2-162">Here is a JSON representation of the resource.</span></span>
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







