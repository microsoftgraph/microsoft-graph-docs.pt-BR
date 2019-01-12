---
title: Excluir windows10CompliancePolicy
description: Exclui windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 674580b2cff53a75175d1a0a14a2f9620ebf7441
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964253"
---
# <a name="delete-windows10compliancepolicy"></a><span data-ttu-id="2d905-103">Excluir windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2d905-103">Delete windows10CompliancePolicy</span></span>

> <span data-ttu-id="2d905-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d905-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d905-105">Exclui [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2d905-105">Deletes a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d905-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d905-106">Prerequisites</span></span>
<span data-ttu-id="2d905-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d905-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d905-109">Permission type</span></span>|<span data-ttu-id="2d905-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d905-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d905-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d905-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d905-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d905-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d905-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d905-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d905-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d905-114">Not supported.</span></span>|
|<span data-ttu-id="2d905-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d905-115">Application</span></span>|<span data-ttu-id="2d905-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d905-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d905-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d905-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2d905-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d905-118">Request headers</span></span>
|<span data-ttu-id="2d905-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d905-119">Header</span></span>|<span data-ttu-id="2d905-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2d905-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d905-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d905-121">Authorization</span></span>|<span data-ttu-id="2d905-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d905-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d905-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d905-123">Accept</span></span>|<span data-ttu-id="2d905-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d905-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d905-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d905-125">Request body</span></span>
<span data-ttu-id="2d905-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d905-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d905-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d905-127">Response</span></span>
<span data-ttu-id="2d905-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d905-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2d905-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d905-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d905-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d905-130">Request</span></span>
<span data-ttu-id="2d905-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d905-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2d905-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d905-132">Response</span></span>
<span data-ttu-id="2d905-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



