---
title: Excluir windowsPhone81CompliancePolicy
description: Exclui windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aec94161fcc5211a92a1ef8fe4c6ef59883a6646
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255686"
---
# <a name="delete-windowsphone81compliancepolicy"></a><span data-ttu-id="a3035-103">Excluir windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a3035-103">Delete windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="a3035-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3035-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3035-105">Exclui [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3035-105">Deletes a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3035-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3035-106">Prerequisites</span></span>
<span data-ttu-id="a3035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3035-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3035-109">Permission type</span></span>|<span data-ttu-id="a3035-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3035-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3035-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3035-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3035-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3035-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3035-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3035-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3035-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3035-114">Not supported.</span></span>|
|<span data-ttu-id="a3035-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3035-115">Application</span></span>|<span data-ttu-id="a3035-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3035-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3035-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3035-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a3035-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3035-118">Request headers</span></span>
|<span data-ttu-id="a3035-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3035-119">Header</span></span>|<span data-ttu-id="a3035-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a3035-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3035-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3035-121">Authorization</span></span>|<span data-ttu-id="a3035-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3035-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3035-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3035-123">Accept</span></span>|<span data-ttu-id="a3035-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3035-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3035-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3035-125">Request body</span></span>
<span data-ttu-id="a3035-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3035-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3035-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3035-127">Response</span></span>
<span data-ttu-id="a3035-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3035-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3035-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3035-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3035-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3035-130">Request</span></span>
<span data-ttu-id="a3035-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3035-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a3035-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3035-132">Response</span></span>
<span data-ttu-id="a3035-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3035-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



