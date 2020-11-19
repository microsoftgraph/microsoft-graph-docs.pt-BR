---
title: Ação beginOnboarding
description: Uma solicitação para iniciar a integração.  Deve ser associado às informações de conta do TeamViewer apropriadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78b4dd2aea5b1cfc508f3ffc715a7ef954d152db
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304333"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="23daa-104">Ação beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="23daa-104">beginOnboarding action</span></span>

<span data-ttu-id="23daa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23daa-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23daa-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23daa-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23daa-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23daa-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23daa-108">Uma solicitação para iniciar a integração.</span><span class="sxs-lookup"><span data-stu-id="23daa-108">A request to start onboarding.</span></span>  <span data-ttu-id="23daa-109">Deve ser associado às informações de conta do TeamViewer apropriadas</span><span class="sxs-lookup"><span data-stu-id="23daa-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23daa-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23daa-110">Prerequisites</span></span>
<span data-ttu-id="23daa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23daa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23daa-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23daa-113">Permission type</span></span>|<span data-ttu-id="23daa-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23daa-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23daa-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23daa-115">Delegated (work or school account)</span></span>|<span data-ttu-id="23daa-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23daa-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23daa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23daa-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23daa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23daa-118">Not supported.</span></span>|
|<span data-ttu-id="23daa-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23daa-119">Application</span></span>|<span data-ttu-id="23daa-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23daa-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23daa-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23daa-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="23daa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23daa-122">Request headers</span></span>
|<span data-ttu-id="23daa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23daa-123">Header</span></span>|<span data-ttu-id="23daa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="23daa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23daa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="23daa-125">Authorization</span></span>|<span data-ttu-id="23daa-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23daa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23daa-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23daa-127">Accept</span></span>|<span data-ttu-id="23daa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="23daa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23daa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23daa-129">Request body</span></span>
<span data-ttu-id="23daa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23daa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23daa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="23daa-131">Response</span></span>
<span data-ttu-id="23daa-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23daa-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23daa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23daa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="23daa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23daa-134">Request</span></span>
<span data-ttu-id="23daa-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23daa-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="23daa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="23daa-136">Response</span></span>
<span data-ttu-id="23daa-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23daa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




