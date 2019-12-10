---
title: ação approveApps
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 65f7dc0ddb331af74498c3b14c2b276c77399313
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39927500"
---
# <a name="approveapps-action"></a><span data-ttu-id="f55ca-103">ação approveApps</span><span class="sxs-lookup"><span data-stu-id="f55ca-103">approveApps action</span></span>

> <span data-ttu-id="f55ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f55ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f55ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f55ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f55ca-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f55ca-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f55ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f55ca-107">Prerequisites</span></span>
<span data-ttu-id="f55ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f55ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f55ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f55ca-110">Permission type</span></span>|<span data-ttu-id="f55ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f55ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f55ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f55ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f55ca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f55ca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f55ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f55ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f55ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f55ca-115">Not supported.</span></span>|
|<span data-ttu-id="f55ca-116">Application</span><span class="sxs-lookup"><span data-stu-id="f55ca-116">Application</span></span>|<span data-ttu-id="f55ca-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f55ca-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f55ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f55ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps
```

## <a name="request-headers"></a><span data-ttu-id="f55ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f55ca-119">Request headers</span></span>
|<span data-ttu-id="f55ca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f55ca-120">Header</span></span>|<span data-ttu-id="f55ca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f55ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f55ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f55ca-122">Authorization</span></span>|<span data-ttu-id="f55ca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f55ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f55ca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f55ca-124">Accept</span></span>|<span data-ttu-id="f55ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f55ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f55ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f55ca-126">Request body</span></span>
<span data-ttu-id="f55ca-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f55ca-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f55ca-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f55ca-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f55ca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f55ca-129">Property</span></span>|<span data-ttu-id="f55ca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f55ca-130">Type</span></span>|<span data-ttu-id="f55ca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f55ca-132">packageIds</span><span class="sxs-lookup"><span data-stu-id="f55ca-132">packageIds</span></span>|<span data-ttu-id="f55ca-133">String collection</span><span class="sxs-lookup"><span data-stu-id="f55ca-133">String collection</span></span>|<span data-ttu-id="f55ca-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f55ca-134">Not yet documented</span></span>|
|<span data-ttu-id="f55ca-135">approveAllPermissions</span><span class="sxs-lookup"><span data-stu-id="f55ca-135">approveAllPermissions</span></span>|<span data-ttu-id="f55ca-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="f55ca-136">Boolean</span></span>|<span data-ttu-id="f55ca-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f55ca-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f55ca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55ca-138">Response</span></span>
<span data-ttu-id="f55ca-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f55ca-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f55ca-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f55ca-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f55ca-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f55ca-141">Request</span></span>
<span data-ttu-id="f55ca-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f55ca-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps

Content-type: application/json
Content-length: 87

{
  "packageIds": [
    "Package Ids value"
  ],
  "approveAllPermissions": true
}
```

### <a name="response"></a><span data-ttu-id="f55ca-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55ca-143">Response</span></span>
<span data-ttu-id="f55ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f55ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





