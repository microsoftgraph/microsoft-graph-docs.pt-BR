---
title: função getLicensesForApp
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b18493b4b304ef9ad6afc64c213ae257f0aac054
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461680"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="68d58-103">função getLicensesForApp</span><span class="sxs-lookup"><span data-stu-id="68d58-103">getLicensesForApp function</span></span>

<span data-ttu-id="68d58-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68d58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68d58-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68d58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68d58-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68d58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68d58-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68d58-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68d58-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68d58-108">Prerequisites</span></span>
<span data-ttu-id="68d58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68d58-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68d58-111">Permission type</span></span>|<span data-ttu-id="68d58-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68d58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68d58-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68d58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68d58-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="68d58-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="68d58-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68d58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68d58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68d58-116">Not supported.</span></span>|
|<span data-ttu-id="68d58-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68d58-117">Application</span></span>|<span data-ttu-id="68d58-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="68d58-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68d58-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68d58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="68d58-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68d58-120">Request headers</span></span>
|<span data-ttu-id="68d58-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68d58-121">Header</span></span>|<span data-ttu-id="68d58-122">Valor</span><span class="sxs-lookup"><span data-stu-id="68d58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68d58-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="68d58-123">Authorization</span></span>|<span data-ttu-id="68d58-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68d58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68d58-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68d58-125">Accept</span></span>|<span data-ttu-id="68d58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68d58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68d58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68d58-127">Request body</span></span>
<span data-ttu-id="68d58-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="68d58-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="68d58-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="68d58-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="68d58-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68d58-130">Property</span></span>|<span data-ttu-id="68d58-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="68d58-131">Type</span></span>|<span data-ttu-id="68d58-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="68d58-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68d58-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="68d58-133">bundleId</span></span>|<span data-ttu-id="68d58-134">String</span><span class="sxs-lookup"><span data-stu-id="68d58-134">String</span></span>|<span data-ttu-id="68d58-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68d58-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="68d58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="68d58-136">Response</span></span>
<span data-ttu-id="68d58-137">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68d58-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68d58-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68d58-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="68d58-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68d58-139">Request</span></span>
<span data-ttu-id="68d58-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68d58-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="68d58-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="68d58-141">Response</span></span>
<span data-ttu-id="68d58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68d58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": [
    {
      "@odata.type": "microsoft.graph.vppTokenLicenseSummary",
      "vppTokenId": "Vpp Token Id value",
      "appleId": "Apple Id value",
      "organizationName": "Organization Name value",
      "availableLicenseCount": 5,
      "usedLicenseCount": 0
    }
  ]
}
```





