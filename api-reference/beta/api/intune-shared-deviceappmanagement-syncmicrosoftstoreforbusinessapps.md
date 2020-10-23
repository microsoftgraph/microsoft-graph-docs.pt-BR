---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: daa78a79bc7f174fad2d95cd83376af2b5a131a8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685027"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="63422-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="63422-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="63422-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63422-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63422-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63422-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63422-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63422-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63422-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63422-108">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="63422-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63422-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63422-109">Prerequisites</span></span>
<span data-ttu-id="63422-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63422-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63422-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63422-112">Permission type</span></span>|<span data-ttu-id="63422-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63422-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63422-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63422-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="63422-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="63422-115">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="63422-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63422-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63422-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63422-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63422-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63422-118">Not supported.</span></span>|
|<span data-ttu-id="63422-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63422-119">Application</span></span>||
| <span data-ttu-id="63422-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="63422-120">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="63422-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63422-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63422-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63422-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="63422-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63422-123">Request headers</span></span>
|<span data-ttu-id="63422-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63422-124">Header</span></span>|<span data-ttu-id="63422-125">Valor</span><span class="sxs-lookup"><span data-stu-id="63422-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63422-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="63422-126">Authorization</span></span>|<span data-ttu-id="63422-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63422-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63422-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63422-128">Accept</span></span>|<span data-ttu-id="63422-129">application/json</span><span class="sxs-lookup"><span data-stu-id="63422-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63422-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63422-130">Request body</span></span>
<span data-ttu-id="63422-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63422-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63422-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="63422-132">Response</span></span>
<span data-ttu-id="63422-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63422-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63422-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63422-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="63422-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63422-135">Request</span></span>
<span data-ttu-id="63422-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63422-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="63422-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="63422-137">Response</span></span>
<span data-ttu-id="63422-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63422-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











