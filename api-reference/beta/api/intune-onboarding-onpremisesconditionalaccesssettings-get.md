---
title: Obter onPremisesConditionalAccessSettings
description: Ler propriedades e relações do objeto onPremisesConditionalAccessSettings.
ms.openlocfilehash: 3cc90209a55fc051266f29decfd21a25ce43aa44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032944"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="977fe-103">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="977fe-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="977fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="977fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="977fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="977fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="977fe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="977fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="977fe-107">Ler propriedades e relações do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="977fe-107">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="977fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="977fe-108">Prerequisites</span></span>
<span data-ttu-id="977fe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="977fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="977fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="977fe-111">Permission type</span></span>|<span data-ttu-id="977fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="977fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="977fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="977fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="977fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="977fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="977fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="977fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="977fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="977fe-116">Not supported.</span></span>|
|<span data-ttu-id="977fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="977fe-117">Application</span></span>|<span data-ttu-id="977fe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="977fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="977fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="977fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="977fe-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="977fe-120">Optional query parameters</span></span>
<span data-ttu-id="977fe-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="977fe-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="977fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="977fe-122">Request headers</span></span>
|<span data-ttu-id="977fe-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="977fe-123">Header</span></span>|<span data-ttu-id="977fe-124">Valor</span><span class="sxs-lookup"><span data-stu-id="977fe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="977fe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="977fe-125">Authorization</span></span>|<span data-ttu-id="977fe-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="977fe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="977fe-127">Accept</span><span class="sxs-lookup"><span data-stu-id="977fe-127">Accept</span></span>|<span data-ttu-id="977fe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="977fe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="977fe-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="977fe-129">Request body</span></span>
<span data-ttu-id="977fe-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="977fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="977fe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="977fe-131">Response</span></span>
<span data-ttu-id="977fe-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="977fe-132">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="977fe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="977fe-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="977fe-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="977fe-134">Request</span></span>
<span data-ttu-id="977fe-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="977fe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="977fe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="977fe-136">Response</span></span>
<span data-ttu-id="977fe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="977fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```





