---
title: Excluir localizedNotificationMessage
description: Exclui localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de929d44a79dcd26bb872b138817b7042ea16eb3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262620"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="ebcca-103">Excluir localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="ebcca-103">Delete localizedNotificationMessage</span></span>

<span data-ttu-id="ebcca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebcca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebcca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebcca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebcca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebcca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebcca-107">Exclui [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="ebcca-107">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebcca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebcca-108">Prerequisites</span></span>
<span data-ttu-id="ebcca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebcca-111">Permission type</span></span>|<span data-ttu-id="ebcca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebcca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebcca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebcca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebcca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebcca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebcca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebcca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcca-116">Not supported.</span></span>|
|<span data-ttu-id="ebcca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebcca-117">Application</span></span>|<span data-ttu-id="ebcca-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcca-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebcca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="ebcca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcca-120">Request headers</span></span>
|<span data-ttu-id="ebcca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebcca-121">Header</span></span>|<span data-ttu-id="ebcca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebcca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebcca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebcca-123">Authorization</span></span>|<span data-ttu-id="ebcca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebcca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebcca-125">Accept</span></span>|<span data-ttu-id="ebcca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebcca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcca-127">Request body</span></span>
<span data-ttu-id="ebcca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebcca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebcca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcca-129">Response</span></span>
<span data-ttu-id="ebcca-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebcca-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebcca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebcca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebcca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcca-132">Request</span></span>
<span data-ttu-id="ebcca-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebcca-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="ebcca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcca-134">Response</span></span>
<span data-ttu-id="ebcca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebcca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




