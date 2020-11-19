---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35fc1ebb54ce7dc66fcc8cfede7e43fe8d9a6821
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304032"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="90c1e-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="90c1e-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="90c1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90c1e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90c1e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90c1e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90c1e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90c1e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90c1e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c1e-108">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="90c1e-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90c1e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90c1e-109">Prerequisites</span></span>
<span data-ttu-id="90c1e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c1e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90c1e-112">Permission type</span></span>|<span data-ttu-id="90c1e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90c1e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c1e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90c1e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="90c1e-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="90c1e-115">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="90c1e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c1e-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90c1e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90c1e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c1e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90c1e-118">Not supported.</span></span>|
|<span data-ttu-id="90c1e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c1e-119">Application</span></span>||
| <span data-ttu-id="90c1e-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="90c1e-120">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="90c1e-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c1e-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c1e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90c1e-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="90c1e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90c1e-123">Request headers</span></span>
|<span data-ttu-id="90c1e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90c1e-124">Header</span></span>|<span data-ttu-id="90c1e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="90c1e-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c1e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="90c1e-126">Authorization</span></span>|<span data-ttu-id="90c1e-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90c1e-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c1e-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90c1e-128">Accept</span></span>|<span data-ttu-id="90c1e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="90c1e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c1e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90c1e-130">Request body</span></span>
<span data-ttu-id="90c1e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90c1e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c1e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c1e-132">Response</span></span>
<span data-ttu-id="90c1e-133">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90c1e-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90c1e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90c1e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="90c1e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90c1e-135">Request</span></span>
<span data-ttu-id="90c1e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90c1e-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="90c1e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c1e-137">Response</span></span>
<span data-ttu-id="90c1e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90c1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










