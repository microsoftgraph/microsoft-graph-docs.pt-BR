---
title: função getLicensesForApp
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42b26bcd7e93a285a3ab4169787d9b230132bd00
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802675"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="02175-103">função getLicensesForApp</span><span class="sxs-lookup"><span data-stu-id="02175-103">getLicensesForApp function</span></span>

> <span data-ttu-id="02175-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02175-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02175-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02175-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02175-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="02175-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02175-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02175-107">Prerequisites</span></span>
<span data-ttu-id="02175-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02175-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02175-110">Permission type</span></span>|<span data-ttu-id="02175-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02175-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02175-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02175-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02175-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02175-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="02175-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02175-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02175-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02175-115">Not supported.</span></span>|
|<span data-ttu-id="02175-116">Application</span><span class="sxs-lookup"><span data-stu-id="02175-116">Application</span></span>|<span data-ttu-id="02175-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02175-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02175-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02175-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="02175-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02175-119">Request headers</span></span>
|<span data-ttu-id="02175-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02175-120">Header</span></span>|<span data-ttu-id="02175-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02175-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02175-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02175-122">Authorization</span></span>|<span data-ttu-id="02175-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02175-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02175-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02175-124">Accept</span></span>|<span data-ttu-id="02175-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02175-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02175-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02175-126">Request body</span></span>
<span data-ttu-id="02175-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="02175-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="02175-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="02175-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="02175-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02175-129">Property</span></span>|<span data-ttu-id="02175-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02175-130">Type</span></span>|<span data-ttu-id="02175-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02175-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02175-132">bundleId</span><span class="sxs-lookup"><span data-stu-id="02175-132">bundleId</span></span>|<span data-ttu-id="02175-133">String</span><span class="sxs-lookup"><span data-stu-id="02175-133">String</span></span>|<span data-ttu-id="02175-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="02175-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="02175-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="02175-135">Response</span></span>
<span data-ttu-id="02175-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02175-136">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02175-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02175-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="02175-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02175-138">Request</span></span>
<span data-ttu-id="02175-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02175-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="02175-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="02175-140">Response</span></span>
<span data-ttu-id="02175-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02175-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




