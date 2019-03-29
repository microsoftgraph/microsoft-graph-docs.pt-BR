---
title: Excluir notificationMessageTemplate
description: Exclui notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82daf5594d7d2b6a2fbad87a09178b64a529d04
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958456"
---
# <a name="delete-notificationmessagetemplate"></a><span data-ttu-id="fbeea-103">Excluir notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="fbeea-103">Delete notificationMessageTemplate</span></span>

> <span data-ttu-id="fbeea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbeea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbeea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbeea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbeea-106">Exclui [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="fbeea-106">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbeea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbeea-107">Prerequisites</span></span>
<span data-ttu-id="fbeea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbeea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbeea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbeea-110">Permission type</span></span>|<span data-ttu-id="fbeea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbeea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbeea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbeea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbeea-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbeea-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbeea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbeea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbeea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbeea-115">Not supported.</span></span>|
|<span data-ttu-id="fbeea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbeea-116">Application</span></span>|<span data-ttu-id="fbeea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbeea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbeea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbeea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="fbeea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbeea-119">Request headers</span></span>
|<span data-ttu-id="fbeea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbeea-120">Header</span></span>|<span data-ttu-id="fbeea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fbeea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbeea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbeea-122">Authorization</span></span>|<span data-ttu-id="fbeea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbeea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbeea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbeea-124">Accept</span></span>|<span data-ttu-id="fbeea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbeea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbeea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbeea-126">Request body</span></span>
<span data-ttu-id="fbeea-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbeea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbeea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbeea-128">Response</span></span>
<span data-ttu-id="fbeea-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fbeea-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fbeea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbeea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbeea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbeea-131">Request</span></span>
<span data-ttu-id="fbeea-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbeea-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="fbeea-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbeea-133">Response</span></span>
<span data-ttu-id="fbeea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbeea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




