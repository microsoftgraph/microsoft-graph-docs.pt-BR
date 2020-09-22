---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6594e67b2147594c941e29cf9662d3f18de0ae4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011134"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="64698-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="64698-103">getUserIdsWithFlaggedAppRegistration function</span></span>

<span data-ttu-id="64698-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="64698-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64698-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64698-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64698-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64698-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64698-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64698-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64698-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64698-108">Prerequisites</span></span>
<span data-ttu-id="64698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64698-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64698-111">Permission type</span></span>|<span data-ttu-id="64698-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64698-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64698-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64698-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64698-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64698-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64698-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64698-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64698-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64698-116">Not supported.</span></span>|
|<span data-ttu-id="64698-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64698-117">Application</span></span>|<span data-ttu-id="64698-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64698-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64698-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64698-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="64698-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64698-120">Request headers</span></span>
|<span data-ttu-id="64698-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64698-121">Header</span></span>|<span data-ttu-id="64698-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64698-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64698-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64698-123">Authorization</span></span>|<span data-ttu-id="64698-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64698-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64698-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64698-125">Accept</span></span>|<span data-ttu-id="64698-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64698-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64698-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64698-127">Request body</span></span>
<span data-ttu-id="64698-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64698-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64698-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64698-129">Response</span></span>
<span data-ttu-id="64698-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64698-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64698-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64698-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64698-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64698-132">Request</span></span>
<span data-ttu-id="64698-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64698-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="64698-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="64698-134">Response</span></span>
<span data-ttu-id="64698-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64698-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```






