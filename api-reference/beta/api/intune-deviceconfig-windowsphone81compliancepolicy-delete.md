---
title: Excluir windowsPhone81CompliancePolicy
description: Exclui windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b513f414cb4dcce591ce36bb474a23f3a56d0d9e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230041"
---
# <a name="delete-windowsphone81compliancepolicy"></a><span data-ttu-id="ea9db-103">Excluir windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ea9db-103">Delete windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="ea9db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea9db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea9db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea9db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea9db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea9db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea9db-107">Exclui [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ea9db-107">Deletes a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea9db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea9db-108">Prerequisites</span></span>
<span data-ttu-id="ea9db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea9db-111">Permission type</span></span>|<span data-ttu-id="ea9db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea9db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea9db-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea9db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea9db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea9db-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea9db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea9db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea9db-116">Not supported.</span></span>|
|<span data-ttu-id="ea9db-117">Application</span><span class="sxs-lookup"><span data-stu-id="ea9db-117">Application</span></span>|<span data-ttu-id="ea9db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea9db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea9db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ea9db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9db-120">Request headers</span></span>
|<span data-ttu-id="ea9db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea9db-121">Header</span></span>|<span data-ttu-id="ea9db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea9db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea9db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea9db-123">Authorization</span></span>|<span data-ttu-id="ea9db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea9db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea9db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea9db-125">Accept</span></span>|<span data-ttu-id="ea9db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea9db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea9db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9db-127">Request body</span></span>
<span data-ttu-id="ea9db-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea9db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea9db-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9db-129">Response</span></span>
<span data-ttu-id="ea9db-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea9db-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea9db-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea9db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea9db-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9db-132">Request</span></span>
<span data-ttu-id="ea9db-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea9db-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ea9db-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9db-134">Response</span></span>
<span data-ttu-id="ea9db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea9db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




