---
title: ação connect
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8acaa40e29e76dfd0d71652339664688a0147cf6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665659"
---
# <a name="connect-action"></a><span data-ttu-id="c8af8-103">ação connect</span><span class="sxs-lookup"><span data-stu-id="c8af8-103">connect action</span></span>

<span data-ttu-id="c8af8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8af8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8af8-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8af8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8af8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8af8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8af8-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8af8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8af8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8af8-108">Prerequisites</span></span>
<span data-ttu-id="c8af8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8af8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8af8-111">Permission type</span></span>|<span data-ttu-id="c8af8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8af8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8af8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8af8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8af8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8af8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8af8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8af8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8af8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8af8-116">Not supported.</span></span>|
|<span data-ttu-id="c8af8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8af8-117">Application</span></span>|<span data-ttu-id="c8af8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8af8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8af8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8af8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings/connect
```

## <a name="request-headers"></a><span data-ttu-id="c8af8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8af8-120">Request headers</span></span>
|<span data-ttu-id="c8af8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8af8-121">Header</span></span>|<span data-ttu-id="c8af8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8af8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8af8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8af8-123">Authorization</span></span>|<span data-ttu-id="c8af8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8af8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8af8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8af8-125">Accept</span></span>|<span data-ttu-id="c8af8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8af8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8af8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8af8-127">Request body</span></span>
<span data-ttu-id="c8af8-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c8af8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c8af8-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c8af8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c8af8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8af8-130">Property</span></span>|<span data-ttu-id="c8af8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8af8-131">Type</span></span>|<span data-ttu-id="c8af8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8af8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8af8-133">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8af8-133">ownerUserPrincipalName</span></span>|<span data-ttu-id="c8af8-134">String</span><span class="sxs-lookup"><span data-stu-id="c8af8-134">String</span></span>|<span data-ttu-id="c8af8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8af8-135">Not yet documented</span></span>|
|<span data-ttu-id="c8af8-136">serviceAccountCredentials</span><span class="sxs-lookup"><span data-stu-id="c8af8-136">serviceAccountCredentials</span></span>|<span data-ttu-id="c8af8-137">String</span><span class="sxs-lookup"><span data-stu-id="c8af8-137">String</span></span>|<span data-ttu-id="c8af8-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8af8-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c8af8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8af8-139">Response</span></span>
<span data-ttu-id="c8af8-140">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8af8-140">If successful, this action returns a `200 OK` response code and a [chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8af8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8af8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8af8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8af8-142">Request</span></span>
<span data-ttu-id="c8af8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8af8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/connect

Content-type: application/json
Content-length: 136

{
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "serviceAccountCredentials": "Service Account Credentials value"
}
```

### <a name="response"></a><span data-ttu-id="c8af8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8af8-144">Response</span></span>
<span data-ttu-id="c8af8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8af8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 29

{
  "value": "inprogress"
}
```




