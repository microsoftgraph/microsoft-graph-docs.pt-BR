---
title: Excluir deviceComplianceActionItem
description: Exclui deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189152018478877b4ee61f437f1c160d0fad1234
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572679"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="6d292-103">Excluir deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="6d292-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="6d292-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d292-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d292-105">Exclui [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6d292-105">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d292-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d292-106">Prerequisites</span></span>
<span data-ttu-id="6d292-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d292-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d292-109">Permission type</span></span>|<span data-ttu-id="6d292-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d292-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d292-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d292-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d292-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d292-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d292-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d292-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d292-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d292-114">Not supported.</span></span>|
|<span data-ttu-id="6d292-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d292-115">Application</span></span>|<span data-ttu-id="6d292-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d292-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d292-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d292-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="6d292-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d292-118">Request headers</span></span>
|<span data-ttu-id="6d292-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d292-119">Header</span></span>|<span data-ttu-id="6d292-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6d292-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d292-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d292-121">Authorization</span></span>|<span data-ttu-id="6d292-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d292-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d292-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d292-123">Accept</span></span>|<span data-ttu-id="6d292-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d292-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d292-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d292-125">Request body</span></span>
<span data-ttu-id="6d292-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d292-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d292-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d292-127">Response</span></span>
<span data-ttu-id="6d292-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d292-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d292-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d292-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d292-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d292-130">Request</span></span>
<span data-ttu-id="6d292-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d292-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="6d292-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d292-132">Response</span></span>
<span data-ttu-id="6d292-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



