---
title: função getLicensesForApp
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a568350cacac5ca640857aeaa8fb6f6d91e5b3fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831469"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="9c01f-103">função getLicensesForApp</span><span class="sxs-lookup"><span data-stu-id="9c01f-103">getLicensesForApp function</span></span>

> <span data-ttu-id="9c01f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c01f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c01f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c01f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c01f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c01f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c01f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c01f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c01f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c01f-108">Prerequisites</span></span>
<span data-ttu-id="9c01f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c01f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c01f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c01f-111">Permission type</span></span>|<span data-ttu-id="9c01f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c01f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c01f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c01f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c01f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c01f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c01f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c01f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c01f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c01f-116">Not supported.</span></span>|
|<span data-ttu-id="9c01f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c01f-117">Application</span></span>|<span data-ttu-id="9c01f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c01f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c01f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c01f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="9c01f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c01f-120">Request headers</span></span>
|<span data-ttu-id="9c01f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c01f-121">Header</span></span>|<span data-ttu-id="9c01f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9c01f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c01f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c01f-123">Authorization</span></span>|<span data-ttu-id="9c01f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c01f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c01f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c01f-125">Accept</span></span>|<span data-ttu-id="9c01f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c01f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c01f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c01f-127">Request body</span></span>
<span data-ttu-id="9c01f-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9c01f-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9c01f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9c01f-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9c01f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c01f-130">Property</span></span>|<span data-ttu-id="9c01f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c01f-131">Type</span></span>|<span data-ttu-id="9c01f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c01f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c01f-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="9c01f-133">bundleId</span></span>|<span data-ttu-id="9c01f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c01f-134">String</span></span>|<span data-ttu-id="9c01f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c01f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c01f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c01f-136">Response</span></span>
<span data-ttu-id="9c01f-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c01f-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c01f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c01f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c01f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c01f-139">Request</span></span>
<span data-ttu-id="9c01f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c01f-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9c01f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c01f-141">Response</span></span>
<span data-ttu-id="9c01f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c01f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





