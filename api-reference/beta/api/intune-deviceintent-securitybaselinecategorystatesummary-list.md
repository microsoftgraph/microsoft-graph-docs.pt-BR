---
title: Listar securityBaselineCategoryStateSummaries
description: Listar Propriedades e relações dos objetos securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a91534f7c7178c548c4bd45119c36fcb2f3911a7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311053"
---
# <a name="list-securitybaselinecategorystatesummaries"></a><span data-ttu-id="79f8c-103">Listar securityBaselineCategoryStateSummaries</span><span class="sxs-lookup"><span data-stu-id="79f8c-103">List securityBaselineCategoryStateSummaries</span></span>

<span data-ttu-id="79f8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79f8c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79f8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79f8c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79f8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79f8c-107">Listar Propriedades e relações dos objetos [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="79f8c-107">List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79f8c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79f8c-108">Prerequisites</span></span>
<span data-ttu-id="79f8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79f8c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79f8c-111">Permission type</span></span>|<span data-ttu-id="79f8c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79f8c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79f8c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79f8c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79f8c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f8c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79f8c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79f8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f8c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79f8c-116">Not supported.</span></span>|
|<span data-ttu-id="79f8c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79f8c-117">Application</span></span>|<span data-ttu-id="79f8c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f8c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79f8c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79f8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="79f8c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79f8c-120">Request headers</span></span>
|<span data-ttu-id="79f8c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79f8c-121">Header</span></span>|<span data-ttu-id="79f8c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79f8c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79f8c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79f8c-123">Authorization</span></span>|<span data-ttu-id="79f8c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79f8c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79f8c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79f8c-125">Accept</span></span>|<span data-ttu-id="79f8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79f8c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f8c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79f8c-127">Request body</span></span>
<span data-ttu-id="79f8c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79f8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79f8c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f8c-129">Response</span></span>
<span data-ttu-id="79f8c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79f8c-130">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f8c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79f8c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79f8c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79f8c-132">Request</span></span>
<span data-ttu-id="79f8c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79f8c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="79f8c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f8c-134">Response</span></span>
<span data-ttu-id="79f8c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79f8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




