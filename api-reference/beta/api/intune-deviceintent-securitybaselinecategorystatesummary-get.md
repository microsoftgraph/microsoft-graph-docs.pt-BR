---
title: Obter securityBaselineCategoryStateSummary
description: Leia as propriedades e as relações do objeto securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15e028e00f66157f21bcdfb2d891e95eba4f1ce1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691726"
---
# <a name="get-securitybaselinecategorystatesummary"></a><span data-ttu-id="906dd-103">Obter securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="906dd-103">Get securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="906dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="906dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="906dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="906dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="906dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="906dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="906dd-107">Leia as propriedades e as relações do objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="906dd-107">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="906dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="906dd-108">Prerequisites</span></span>
<span data-ttu-id="906dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="906dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="906dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="906dd-111">Permission type</span></span>|<span data-ttu-id="906dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="906dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="906dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="906dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="906dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="906dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="906dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="906dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="906dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="906dd-116">Not supported.</span></span>|
|<span data-ttu-id="906dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="906dd-117">Application</span></span>|<span data-ttu-id="906dd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="906dd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="906dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="906dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="906dd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="906dd-120">Optional query parameters</span></span>
<span data-ttu-id="906dd-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="906dd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="906dd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="906dd-122">Request headers</span></span>
|<span data-ttu-id="906dd-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="906dd-123">Header</span></span>|<span data-ttu-id="906dd-124">Valor</span><span class="sxs-lookup"><span data-stu-id="906dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="906dd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="906dd-125">Authorization</span></span>|<span data-ttu-id="906dd-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="906dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="906dd-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="906dd-127">Accept</span></span>|<span data-ttu-id="906dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="906dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="906dd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="906dd-129">Request body</span></span>
<span data-ttu-id="906dd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="906dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="906dd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="906dd-131">Response</span></span>
<span data-ttu-id="906dd-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="906dd-132">If successful, this method returns a `200 OK` response code and [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="906dd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="906dd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="906dd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="906dd-134">Request</span></span>
<span data-ttu-id="906dd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="906dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="906dd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="906dd-136">Response</span></span>
<span data-ttu-id="906dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="906dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": {
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
}
```





