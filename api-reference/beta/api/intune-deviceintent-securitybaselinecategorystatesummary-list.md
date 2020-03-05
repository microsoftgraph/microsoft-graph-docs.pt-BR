---
title: Listar securityBaselineCategoryStateSummaries
description: Listar Propriedades e relações dos objetos securityBaselineCategoryStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c82db6a1b9d53ea2c4480df8d8b692d7a361c47f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470256"
---
# <a name="list-securitybaselinecategorystatesummaries"></a><span data-ttu-id="691d3-103">Listar securityBaselineCategoryStateSummaries</span><span class="sxs-lookup"><span data-stu-id="691d3-103">List securityBaselineCategoryStateSummaries</span></span>

<span data-ttu-id="691d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="691d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="691d3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="691d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="691d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="691d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="691d3-107">Listar Propriedades e relações dos objetos [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="691d3-107">List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="691d3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="691d3-108">Prerequisites</span></span>
<span data-ttu-id="691d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="691d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="691d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="691d3-111">Permission type</span></span>|<span data-ttu-id="691d3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="691d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="691d3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="691d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="691d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="691d3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="691d3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="691d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="691d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="691d3-116">Not supported.</span></span>|
|<span data-ttu-id="691d3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="691d3-117">Application</span></span>|<span data-ttu-id="691d3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="691d3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="691d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="691d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="691d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="691d3-120">Request headers</span></span>
|<span data-ttu-id="691d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="691d3-121">Header</span></span>|<span data-ttu-id="691d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="691d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="691d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="691d3-123">Authorization</span></span>|<span data-ttu-id="691d3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="691d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="691d3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="691d3-125">Accept</span></span>|<span data-ttu-id="691d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="691d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="691d3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="691d3-127">Request body</span></span>
<span data-ttu-id="691d3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="691d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="691d3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="691d3-129">Response</span></span>
<span data-ttu-id="691d3-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="691d3-130">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="691d3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="691d3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="691d3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="691d3-132">Request</span></span>
<span data-ttu-id="691d3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="691d3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="691d3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="691d3-134">Response</span></span>
<span data-ttu-id="691d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="691d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
      "id": "7a650997-0997-7a65-9709-657a9709657a",
      "secureCount": 11,
      "notSecureCount": 14,
      "unknownCount": 12,
      "errorCount": 10,
      "conflictCount": 13,
      "notApplicableCount": 2,
      "displayName": "Display Name value"
    }
  ]
}
```





