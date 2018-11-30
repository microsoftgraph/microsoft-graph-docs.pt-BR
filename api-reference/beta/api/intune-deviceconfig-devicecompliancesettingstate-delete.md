---
title: Excluir deviceComplianceSettingState
description: Exclui deviceComplianceSettingState.
ms.openlocfilehash: 524793c925f4398cb3fcb594354f7fe907e53e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036419"
---
# <a name="delete-devicecompliancesettingstate"></a><span data-ttu-id="3eb2d-103">Excluir deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="3eb2d-103">Delete deviceComplianceSettingState</span></span>

> <span data-ttu-id="3eb2d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb2d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eb2d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3eb2d-107">Exclui [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3eb2d-107">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3eb2d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3eb2d-108">Prerequisites</span></span>
<span data-ttu-id="3eb2d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb2d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eb2d-111">Permission type</span></span>|<span data-ttu-id="3eb2d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3eb2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb2d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eb2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb2d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb2d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb2d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eb2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-116">Not supported.</span></span>|
|<span data-ttu-id="3eb2d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eb2d-117">Application</span></span>|<span data-ttu-id="3eb2d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb2d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eb2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3eb2d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb2d-120">Request headers</span></span>
|<span data-ttu-id="3eb2d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3eb2d-121">Header</span></span>|<span data-ttu-id="3eb2d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3eb2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb2d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eb2d-123">Authorization</span></span>|<span data-ttu-id="3eb2d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb2d-125">Accept</span></span>|<span data-ttu-id="3eb2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb2d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb2d-127">Request body</span></span>
<span data-ttu-id="3eb2d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb2d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb2d-129">Response</span></span>
<span data-ttu-id="3eb2d-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3eb2d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eb2d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3eb2d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb2d-132">Request</span></span>
<span data-ttu-id="3eb2d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="3eb2d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb2d-134">Response</span></span>
<span data-ttu-id="3eb2d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eb2d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





