---
title: Excluir deviceCompliancePolicySettingStateSummary
description: Exclui deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e4b4e732af98c802f7c61a69d1e6c703003d5f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869122"
---
# <a name="delete-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="bbaef-103">Excluir deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="bbaef-103">Delete deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="bbaef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bbaef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbaef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bbaef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbaef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bbaef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbaef-107">Exclui [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bbaef-107">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbaef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbaef-108">Prerequisites</span></span>
<span data-ttu-id="bbaef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbaef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbaef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbaef-111">Permission type</span></span>|<span data-ttu-id="bbaef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbaef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbaef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbaef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbaef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbaef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbaef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbaef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbaef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbaef-116">Not supported.</span></span>|
|<span data-ttu-id="bbaef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbaef-117">Application</span></span>|<span data-ttu-id="bbaef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbaef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbaef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbaef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="bbaef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbaef-120">Request headers</span></span>
|<span data-ttu-id="bbaef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbaef-121">Header</span></span>|<span data-ttu-id="bbaef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbaef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbaef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbaef-123">Authorization</span></span>|<span data-ttu-id="bbaef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbaef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbaef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbaef-125">Accept</span></span>|<span data-ttu-id="bbaef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbaef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbaef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbaef-127">Request body</span></span>
<span data-ttu-id="bbaef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbaef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbaef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbaef-129">Response</span></span>
<span data-ttu-id="bbaef-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbaef-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bbaef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbaef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbaef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbaef-132">Request</span></span>
<span data-ttu-id="bbaef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbaef-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="bbaef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbaef-134">Response</span></span>
<span data-ttu-id="bbaef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbaef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





